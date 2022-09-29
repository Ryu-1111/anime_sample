<template>
<div obu>
<div class="obu_1">
  <v-sheet
  color="blue"
  height="250"
  width="500"
></v-sheet>
</div>
<div class="obu_2">
  <v-sheet
  color="lime"
  height="250"
  width="500"
></v-sheet>
</div>
<div class="obu_3">
  <v-sheet
  color="purple"
  height="250"
  width="500"
></v-sheet>
</div>
<div class="obu_4">
  <v-sheet
  color="teal"
  height="250"
  width="500"
></v-sheet>
</div>
</div>
  </template>
  
  <script>
  import { gsap } from 'gsap';


export default {
  
  mounted() {
    gsap.from(".obu", {
  autoAlpha: 0,
  duration: 1,
  stagger: 2, // 3秒ごとに出現
})
    gsap.to(".obu_1", {
      x: 500, //動かす方向
  duration: 0.5, //秒数
  delay: 2.5, //遅延時間
  rotate: 180, //回転角度
})
gsap.to(".obu_2", {
  x: 500, //動かす方向
  duration: 0.5, //秒数
  delay: 3, //遅延時間
  rotate: 180, //回転角度
})
gsap.to(".obu_3", {
  x: 500, //動かす方向
  duration: 0.5, //秒数
  delay: 3.5, //遅延時間
  rotate: 180, //回転角度
})
gsap.to(".obu_4", {
  x: 500, //動かす方向
  duration: 0.5, //秒数
  delay: 4, //遅延時間
  rotate: 180, //回転角度
})
},

}
  </script>
  
  <style scoped>
  .obu_1 {
    position: absolute;
    top: 25px;
    right: 550px;

    animation: fadein 6s ease-out forwards;
}

@keyframes fadein {
  0% {
    opacity: 0
  }
  100% {
    opacity: 1
  }
  }
  

  .obu_2 {
    position: absolute;
    top: 25px;
    right: 1100px;

    animation: fadein 7s ease-out forwards;
}

@keyframes fadein {
  0% {
    opacity: 0
  }
  100% {
    opacity: 1
  }

  }
  .obu_3 {
    position: absolute;
    top: 325px;
    right: 550px;

    animation: fadein 8s ease-out forwards;
}

@keyframes fadein {
  0% {
    opacity: 0
  }
  100% {
    opacity: 1
  }

  }

  .obu_4 {
    position: absolute;
    top: 325px;
    right: 1100px;

    animation: fadein 9s ease-out forwards;
}

@keyframes fadein {
  0% {
    opacity: 0
  }
  100% {
    opacity: 1
  }

  }
  </style>