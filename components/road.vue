<template>
<div>


<v-flex class="d-flex justify-center pa-16">
<div class="load_a">
    <v-avatar
  color="red"
  size="25"
></v-avatar>
</div>

<div class="load_b">
    <v-avatar
  color="blue"
  size="25"
></v-avatar>
    </div>

<div class="load_c">
    <v-avatar
  color="teal"
  size="25"
></v-avatar>
    </div>
<div class="load_d">
    <v-avatar
  color="yellow"
  size="25"
></v-avatar>
    </div>


<div class="load_e">
  <v-avatar
  color="black"
  size="25"
></v-avatar>
  </div>
  </v-flex>
  </div>
  
</template>

<script>
import { gsap } from 'gsap';


export default {
  
  mounted() {
    
    gsap.to(".load_a", {
  y: -35,
  duration: 0.5,
  repeat: -1, // 無限に繰り返し
  repeatDelay: 0.1, // 繰り返し時に0.5秒の待機,
})
gsap.to(".load_b", {
  y: -35,
  duration: 0.5,
  delay: 0.2,
  repeat: -1, // 無限に繰り返し
  repeatDelay: 0.1, // 繰り返し時に0.5秒の待機,
})
gsap.to(".load_c", {
  y: -35,
  duration: 0.5,
  delay: 0.4,
  repeat: -1, // 無限に繰り返し
  repeatDelay: 0.1, // 繰り返し時に0.5秒の待機,
})
gsap.to(".load_d", {
  y: -35,
  duration: 0.5,
  delay: 0.6,
  repeat: -1, // 無限に繰り返し
  repeatDelay: 0.1, // 繰り返し時に0.5秒の待機,
})
gsap.to(".load_e", {
  y: -35,
  duration: 0.5,
  delay: 0.8,
  repeat: -1, // 無限に繰り返し
  repeatDelay: 0.1, // 繰り返し時に0.5秒の待機,
})
},

}


</script>


<style>
.load_sample {
color: white;

}

.load_a {
  animation: fadeout-anim 2s linear forwards;
}

@keyframes fadeout-anim {
100% {
		opacity: 0;
	}
}

.load_b {
  animation: fadeout-anim 2s linear forwards;
}

@keyframes fadeout-anim {
100% {
		opacity: 0;
	}
}


.load_c {
  animation: fadeout-anim 2s linear forwards;
}

@keyframes fadeout-anim {
100% {
		opacity: 0;
	}
}

.load_d {
  animation: fadeout-anim 2s linear forwards;
}

@keyframes fadeout-anim {
100% {
		opacity: 0;
	}
}

.load_e {
  animation: fadeout-anim 2s linear forwards;
}

@keyframes fadeout-anim {
100% {
		opacity: 0;
	}
}
</style>
