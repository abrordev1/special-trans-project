<template>
  <div class="home-page">
    
    <HeroSection></HeroSection>
    
  </div>
</template>

<script>
import TheButton from '../../ui/TheButton.vue';
import TheTitle from '../../ui/TheTitle.vue';
import HeroSection from './sections/HeroSection.vue'




export default {
  components: { TheButton, TheTitle, HeroSection }
}
</script>
