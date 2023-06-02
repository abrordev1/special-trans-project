<template>
  <div class="home-page">
    <h1>Home page</h1>
    <TheButton>Заказать звонок </TheButton>
    <TheTitle>Почему выбирают нас</TheTitle>
  </div>
</template>

<script>
import TheButton from '../../ui/TheButton.vue';
import TheTitle from '../../ui/TheTitle.vue';



export default {
  components: { TheButton, TheTitle }
}
</script>
