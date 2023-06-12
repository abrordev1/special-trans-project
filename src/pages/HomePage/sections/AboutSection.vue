<template>
    <section class="about pb-16 lg:pb-20">
        <div class="container flex flex-wrap justify-between items-center">
            <div class="wrapper-left lg:w-[50%]">
                <TheTitle>О компании СПЕЦ-ТРАНС</TheTitle>
                <div class="text-sm lg:text-lg text-[#67675F] font-normal leading-6 pt-6 pb-5 lg:pb-0 lg:pt-7">Наша фирма существует уже многие годы, заработав репутацию на рынке предлагаемых услуг
                    как надежного и ответственного партнера. В число наших клиентов вошли крупнейшие организации. При этом
                    стоит отметить, что на индивидуальный подход при заказе наших услуг могут рассчитывать как крупные
                    компании, так и частные лица.</div>
            </div>
            <div class="wrapper-right flex flex-wrap justify-center items-center gap-5 sm:gap-44 w-full lg:w-[50%] h-[340px] lg:h-[446px] bg-[#F8F8F8] rounded-3xl">
                <div class="left">
                    <div class="top flex justify-center gap-0 lg:gap-[10px]">
                        <h2 class="text-[50px] lg:text-[88px] leading-[71px] lg:leading-[124px] text-dark font-semibold lg:font-light pb-2 lg:pb-0">60</h2>
                        <h3 class="text-[#27AE60] font-medium text-[40px] leading-[56px]">+</h3>
                    </div>

                    <p class="text-lg lg:text-2xl leading-[25px] lg:leading-8 text-[#67675F]">Единиц техники</p>
                </div>
                <div class="right text-center">
                    <h2 class="text-[50px] lg:text-[88px] leading-[71px] lg:leading-[124px] text-dark font-semibold lg:font-light pb-2 lg:pb-0">15</h2>
                    <p class="text-lg lg:text-2xl leading-[25px] lg:leading-8 text-[#67675F]">Карьеров</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import TheTitle from '../../../ui/TheTitle.vue';


export default {
    components: { TheTitle }
}


</script>