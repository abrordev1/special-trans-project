<template>
  <div class="home-page">    
    <HeroSection />
    <ServicesSections />
    
  </div>
</template>

<script>

import HeroSection from './sections/HeroSection.vue'
import ServicesSections from './sections/ServicesSections.vue';




export default {
  components: { HeroSection, ServicesSections }
}
</script>
