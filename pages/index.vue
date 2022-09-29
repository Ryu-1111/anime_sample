<template>
<div>
<road/>
<obuje_1/>
</div>

</template>


<script>
import road from "/components/road.vue";
import obuje_1 from "/components/obuje_1.vue";
import { gsap } from 'gsap';

//scrolltriggerも登録する場合は下記
import { ScrollTrigger } from 'gsap/ScrollTrigger';

if (process.client) {
  gsap.registerPlugin(ScrollTrigger)
}

export default {
  components: {
    road,
    obuje_1,
  },
  mounted () {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()

      setTimeout(() => this.$nuxt.$loading.finish(), 500)
    })
  }
  }
  
</script>

<style scoped>

  </style>
  