<template>
  <div class="scenes" ref="scenes">
    <img class="scene-1" :src="img1" alt="" ref="scene1" />
    <img :class="active ? 'active' : ''" class="scene-2" :src="img2" alt="" />
    <img v-if="img3" :src="img3" v-show="active" class="bling" />
  </div>
</template>

<script>
export default {
  name: "CircleTransition",
  components: {},
  props: ["active", "img1", "img2","img3"],
  mounted() {
    setTimeout(() => {
      if (!this.$refs.scenes.offsetHeight || !this.$refs.scenes.offsetWidth) {
        this.$refs.scenes.style.height = this.$refs.scene1.offsetHeight + "px";
        this.$refs.scenes.style.width = this.$refs.scene1.offsetWidth + "px";
      }
    }, 100);
  },
};
</script>

<style scoped>
@property --radius {
  syntax: "<percentage>";
  inherits: true;
  initial-value: -5%;
}
@keyframes scene-transition {
  to {
    --radius: 105%;
  }
}

.scenes {
  position: absolute;
  cursor: pointer;
}
.bling {
  position: absolute;
  width: 100%;
  height: 100%;
  animation: bling 2s infinite linear;
}
@keyframes bling {
  0% {
    opacity: 0.1;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 0.1;
  }
}
.scene-1,
.scene-2 {
  position: absolute;
  object-fit: cover;
}
.scene-2 {
  -webkit-mask-image: radial-gradient(
    circle,
    #fff calc(var(--radius) - 5%),
    transparent calc(var(--radius) + 5%)
  );
}
.active {
  animation: scene-transition 2s linear forwards;
}
</style>
