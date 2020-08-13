<template>
  <div class="home">
    <HeroSlider></HeroSlider> 
    <Service></Service>
    <Recent></Recent>

    
  </div>
</template>

<script>

import HeroSlider from "@/components/HeroSlider.vue";
import Service from "@/components/Service.vue";
import Recent from "@/components/Recent.vue";

  
export default {
  name: "Home",
  components: {
    HeroSlider,
    Service,
    Recent,

  
  },
};
</script>
