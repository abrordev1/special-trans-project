<template>
    <div class="main-materials pb-[60px] lg:pb-[80px]">
        <div class="container">
            <TheTitle>Основные материалы</TheTitle>

            <div class="wrapper flex flex-wrap gap-5 justify-center 2xl:justify-between items-center mt-6 lg:mt-16">
                <MaterialsCard v-for="item in materialsData" :key="item.name" :data="item" />
            </div>
        </div>
    </div>
</template>

<script>
import TheTitle from '../../../ui/TheTitle.vue';
import MaterialsCard from '../components/MaterialsCard.vue';


export default {
    components: { TheTitle, MaterialsCard },
    data() {
        return {
            materialsData: [
                {
                    image: "src/assets/images/material-1.jpg",
                    name: "Песок"
                },
                {
                    image: "src/assets/images/material-2.jpg",
                    name: "Щебень"
                },
                {
                    image: "src/assets/images/material-3.jpg",
                    name: "Асфальтная крошка"
                },
                {
                    image: "src/assets/images/material-4.jpg",
                    name: "Аренда техники"
                },
            ]
        }
    }
}

</script>
