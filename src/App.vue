<template>
  <div class="containner">
    <LineTransitionVue
      @click="active1 = !active1"
      class="msg1"
      :bc="require('@/assets/step1-3.png')"
      :active="active1"
      :content="'嗨，我是大米'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active2 = !active2"
      class="msg2"
      :bc="require('@/assets/step2-3.png')"
      :active="active2"
      :content="'我正在快快长大'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active3 = !active3"
      class="msg3"
      :bc="require('@/assets/step3-3.png')"
      :active="active3"
      :content="'我已经长大了'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active4 = !active4"
      class="msg4"
      :bc="require('@/assets/step4-3.png')"
      :active="active4"
      :content="'我正在清除一些大的杂质'"
    ></LineTransitionVue>
    <!-- <LineTransitionVue
      @click="active4 = !active4"
      class="msg4"
      :bc="require('@/assets/step4-3.png')"
      :active="active4"
      :content="'我正在清除一些大的杂质'"
    ></LineTransitionVue> -->
    <LineTransitionVue
      @click="active5 = !active5"
      class="msg5"
      :bc="require('@/assets/step5-3.png')"
      :active="active5"
      :content="'我正在去除石头，灰尘，杂质'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active6 = !active6"
      class="msg6"
      :bc="require('@/assets/step6-3.png')"
      :active="active6"
      :content="'我正在脱除颖壳'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active7 = !active7"
      class="msg7"
      :bc="require('@/assets/step7-3.png')"
      :active="active7"
      :content="'我在进行加工以及种粮筛选哦'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active8 = !active8"
      class="msg8"
      :bc="require('@/assets/step8-3.png')"
      :active="active8"
      :content="'脱掉米糠的我虽然不怎么好看，但很营养哦'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active9 = !active9"
      class="msg9"
      :bc="require('@/assets/step9-3.png')"
      :active="active9"
      :content="'我的表面杂质被去除了，变得白白的了哟'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active10 = !active10"
      class="msg10"
      :bc="require('@/assets/step10-3.png')"
      :active="active10"
      :content="'把我们按照品质分成等级'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active11 = !active11"
      class="msg11"
      :bc="require('@/assets/step11-3.png')"
      :active="active11"
      :content="'根据我们的颜色进行挑选'"
    ></LineTransitionVue>
    <LineTransitionVue
      @click="active12 = !active12"
      class="msg12"
      :bc="require('@/assets/step12-3.png')"
      :active="active12"
      :content="'我的兄弟姐妹们和我一起装在袋子里'"
    ></LineTransitionVue>

    <CircleTransition
      class="step1"
      :img1="require('@/assets/step1-0.png')"
      :img2="require('@/assets/step1-1.png')"
      :img3="require('@/assets/step1-bling.png')"
      :active="active1"
      @click="active1 = !active1"
    ></CircleTransition>

    <CircleTransition
      class="step2"
      :img1="require('@/assets/step2-0.png')"
      :img2="require('@/assets/step2-1.png')"
      :active="active2"
      @click="active2 = !active2"
    ></CircleTransition>
    <CircleTransition
      class="step3"
      :img1="require('@/assets/step3-0.png')"
      :img2="require('@/assets/step3-1.png')"
      :active="active3"
      @click="active3 = !active3"
    ></CircleTransition>
    <CircleTransition
      class="step4"
      :img1="require('@/assets/step4-0.png')"
      :img2="require('@/assets/step4-1.png')"
      :active="active4"
      @click="active4 = !active4"
    ></CircleTransition>
    <CircleTransition
      class="step5"
      :img1="require('@/assets/step5-0.png')"
      :img2="require('@/assets/step5-1.png')"
      :active="active5"
      @click="active5 = !active5"
    ></CircleTransition>
    <CircleTransition
      class="step6"
      :img1="require('@/assets/step6-0.png')"
      :img2="require('@/assets/step6-1.png')"
      :active="active6"
      @click="active6 = !active6"
    ></CircleTransition>
    <CircleTransition
      class="step7"
      :img1="require('@/assets/step7-0.png')"
      :img2="require('@/assets/step7-1.png')"
      :active="active7"
      @click="active7 = !active7"
    ></CircleTransition>
    <CircleTransition
      class="step8"
      :img1="require('@/assets/step8-0.png')"
      :img2="require('@/assets/step8-1.png')"
      :active="active8"
      @click="active8 = !active8"
    ></CircleTransition>
    <CircleTransition
      class="step9"
      :img1="require('@/assets/step9-0.png')"
      :img2="require('@/assets/step9-1.png')"
      :active="active9"
      @click="active9 = !active9"
    ></CircleTransition>
    <CircleTransition
      class="step10"
      :img1="require('@/assets/step10-0.png')"
      :img2="require('@/assets/step10-1.png')"
      :active="active10"
      @click="active10 = !active10"
    ></CircleTransition>
    <CircleTransition
      class="step11"
      :img1="require('@/assets/step11-0.png')"
      :img2="require('@/assets/step11-1.png')"
      :active="active11"
      @click="active11 = !active11"
    ></CircleTransition>
    <CircleTransition
      class="step12"
      :img1="require('@/assets/step12-0.png')"
      :img2="require('@/assets/step12-1.png')"
      :active="active12"
      @click="active12 = !active12"
    ></CircleTransition>

    <div @click="active1 = !active1" class="title title1">
      <div class="content">胚芽</div>
      <img src="@/assets/step1-2.png" alt="" />
    </div>
    <div @click="active2 = !active2" class="title title2">
      <div class="content">抽穗期</div>
      <img src="@/assets/step2-2.png" alt="" />
    </div>
    <div @click="active3 = !active3" class="title title3">
      <div class="content">机器收割</div>
      <img src="@/assets/step3-2.png" alt="" />
    </div>
    <div @click="active4 = !active4" class="title title4">
      <div class="content">圆筒初轻筛</div>
      <img src="@/assets/step4-2.png" alt="" />
    </div>
    <div @click="active5 = !active5" class="title title5">
      <div class="content">去石</div>
      <img src="@/assets/step5-2.png" alt="" />
    </div>
    <div @click="active6 = !active6" class="title title6">
      <div class="content">砻谷</div>
      <img src="@/assets/step6-2.png" alt="" />
    </div>
    <div @click="active7 = !active7" class="title title7">
      <div class="content">谷糙分离</div>
      <img src="@/assets/step7-2.png" alt="" />
    </div>
    <div @click="active8 = !active8" class="title title8">
      <div class="content">碾米</div>
      <img src="@/assets/step8-2.png" alt="" />
    </div>
    <div @click="active9 = !active9" class="title title9">
      <div class="content">抛光</div>
      <img src="@/assets/step9-2.png" alt="" />
    </div>
    <div @click="active10 = !active10" class="title title10">
      <div class="content">分级</div>
      <img src="@/assets/step10-2.png" alt="" />
    </div>
    <div @click="active11 = !active11" class="title title11">
      <div class="content">色选</div>
      <img src="@/assets/step11-2.png" alt="" />
    </div>
    <div @click="active12 = !active12" class="title title12">
      <div class="content">定量包装</div>
      <img src="@/assets/step12-2.png" alt="" />
    </div>
  </div>
</template>

<script>
import CircleTransition from "./components/CircleTransition.vue";
import LineTransitionVue from "./components/LineTransition.vue";
export default {
  name: "App",
  components: {
    CircleTransition,
    LineTransitionVue,
  },
  data() {
    return {
      active1: false,
      active2: false,
      active3: false,
      active4: false,
      active5: false,
      active6: false,
      active7: false,
      active8: false,
      active9: false,
      active10: false,
      active11: false,
      active12: false,
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
.title12{
  top: 380px;
  left: 45px;
}
.title11{
  top: 910px;
  left: 95px;
}
.title10{
  top: 980px;
  left: 510px;
}
.title9{
  top: 995px;
  left: 820px;
}
.title8{
  top: 995px;
  left: 1150px;
}
.title7{
  top: 970px;
  left: 1360px;
}
.title6{
  top: 910px;
  left: 1660px;
}
.title5{
  top: 285px;
  left: 1720px;
}
.title4{
  top: 75px;
  left: 1250px;
}
.title3{
  top: 20px;
  left: 800px;
}
.title2{
  top: 40px;
  left: 460px;
}
.title1{
  top: 120px;
  left: 140px;
}
.title {
  position: absolute;
  overflow: hidden;
  cursor: pointer;
}
.title .content {
  position: absolute;
  color: #fff;
  font-size: 32px;
  left: 50%;
  transform: translateX(-50%);
  white-space: nowrap;
  padding-left: 65px;
  box-sizing: border-box;
  font-weight: 100;
  bottom: 8px;
}
.msg12 {
  position: absolute;
  left: 360px;
  top: 460px;
}
.step12 {
  position: absolute;
  left: 90px;
  top: 470px;
}
.msg11 {
  position: absolute;
  left: 320px;
  top: 575px;
}
.step11 {
  position: absolute;
  left: 150px;
  top: 670px;
}
.msg10 {
  position: absolute;
  left: 350px;
  top: 660px;
}
.step10 {
  position: absolute;
  left: 420px;
  top: 770px;
}
.msg9 {
  position: absolute;
  left: 650px;
  top: 690px;
}
.step9 {
  position: absolute;
  left: 720px;
  top: 780px;
}
.msg8 {
  position: absolute;
  left: 815px;
  top: 620px;
}
.step8 {
  position: absolute;
  left: 1060px;
  top: 750px;
}
.msg7 {
  position: absolute;
  left: 1250px;
  top: 650px;
}
.step7 {
  position: absolute;
  left: 1360px;
  top: 720px;
}
.msg6 {
  position: absolute;
  left: 1380px;
  top: 565px;
}
.step6 {
  position: absolute;
  left: 1590px;
  top: 650px;
}
.msg5 {
  position: absolute;
  left: 1230px;
  top: 485px;
}
.step5 {
  position: absolute;
  left: 1650px;
  top: 380px;
}
.msg4 {
  position: absolute;
  left: 1200px;
  top: 385px;
}
.step4 {
  position: absolute;
  left: 1350px;
  top: 180px;
}
.msg3 {
  position: absolute;
  left: 960px;
  top: 380px;
}
.step3 {
  position: absolute;
  left: 880px;
  top: 100px;
}
.msg2 {
  position: absolute;
  left: 680px;
  top: 370px;
}
.step2 {
  position: absolute;
  left: 570px;
  top: 110px;
}
.msg1 {
  position: absolute;
  left: 480px;
  top: 370px;
}
.step1 {
  position: absolute;
  left: 290px;
  top: 180px;
}
.containner {
  position: relative;
  width: 1920px;
  height: 1080px;
  background: url(@/assets/0.png);
  overflow: hidden;
}
</style>
