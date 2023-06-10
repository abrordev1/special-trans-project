<template>
  <div class="home-page">    
    <HeroSection />
    <ServicesSections />
    <MainMaterialsSection />
    
  </div>
</template>

<script>

import HeroSection from './sections/HeroSection.vue'
import MainMaterialsSection from './sections/MainMaterialsSection.vue';
import ServicesSections from './sections/ServicesSections.vue';




export default {
  components: { HeroSection, ServicesSections, MainMaterialsSection }
}
</script>
