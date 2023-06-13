<template>
    <div class="wrapper xl:w-[490px] mb-8 xl:mb-0">
        <TheTitle>Остались вопросы?</TheTitle>
        <h3 class="pt-6 pb-2 lg:py-6 text-[#27AE60] text-base lg:text-[28px] leading-[22px] lg:leading-[39px] font-normal">Закажите обратный звонок и узнайте больше о наших услугах!</h3>
        <p class="text-[#67675F] text-sm lg:text-[22px] leading-5 lg:leading-7 font-normal lg:font-light pb-8 lg:pb-[53px]">Оставьте заявку и наш менеджер перезвонит вам в течении 10 минут</p>
        <TheButton class="hidden lg:block">Заказать звонок</TheButton>
    </div>

</template>

<script>
import TheButton from '../../ui/TheButton.vue';
import TheTitle from '../../ui/TheTitle.vue';


export default {
    components: { TheTitle, TheButton }
}

</script>