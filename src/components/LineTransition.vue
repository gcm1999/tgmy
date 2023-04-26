<template>
  <div ref="light" :class="active ? 'light-active' : ''" class="light">
    <div ref="mask" :class="active ? 'active' : ''" class="mask">
      {{ content }}
    </div>
    <img ref="bg" :src="bc" alt="" />
  </div>
</template>

<script>
import { nextTick } from "vue";
export default {
  // data() {},
  props: ["active", "bc", "content"],
  created() {},
  mounted() {
    nextTick(() => {
      console.log(222);
    });

    setTimeout(() => {
    if (
      this.$refs.light.offsetHeight == 0 ||
      this.$refs.light.offsetWidth == 0
    ) {
      this.$refs.mask.style.height = this.$refs.bg.offsetHeight + "px";
      this.$refs.mask.style.width = this.$refs.bg.offsetWidth + "px";
      this.$refs.light.style.height = this.$refs.bg.offsetHeight + "px";
      this.$refs.light.style.width = this.$refs.bg.offsetWidth + "px";
      // console.log( this.$refs.mask.style.height);
      // console.log( this.$refs.mask.style.width);
      console.log(111);
    }
    }, 100);
  },
  methods: {},
};
</script>

<style scoped>
.light {
  /* width: 200px;
  height: 50px; */
  position: absolute;
  cursor: pointer;
}
img {
  position: absolute;
  left: 0;
  top: 0;
  z-index: 1;
}
.mask {
  position: absolute;
  z-index: 2;
  mask-image: linear-gradient(to left, transparent 47.5%, #fff 52.5%);
  mask-size: 210% 90%;
  mask-position: right;
  font-size: 18px;
  color: #000;
  display: flex;
  align-items: center;
  justify-content: center;
}
.active {
  mask-position: left;
  transition: all 2s ease-out;
}
</style>
