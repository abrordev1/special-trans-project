<template>
  <div class="home-page">    
    <HeroSection />
    <ServicesSections />
    <MainMaterialsSection />
    <AboutSection />
    <QestionsSection />
    
  </div>
</template>

<script>

import AboutSection from './sections/AboutSection.vue';
import HeroSection from './sections/HeroSection.vue'
import MainMaterialsSection from './sections/MainMaterialsSection.vue';
import ServicesSections from './sections/ServicesSections.vue';
import QestionsSection from '../../components/QestionsSection.vue';






export default {
  components: { HeroSection, ServicesSections, MainMaterialsSection, AboutSection, QestionsSection },
  
}
</script>
