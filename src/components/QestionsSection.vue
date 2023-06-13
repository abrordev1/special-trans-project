<template>
    <section class="questions bg-[#F8F8F8] py-16 xl:py-0">
        <div class="container flex flex-wrap justify-between items-center">
            <Questions />
            <Registration />
        </div>

    </section>
</template>

<script>
import Questions from './sectionComponents/questions.vue';
import Registration from './sectionComponents/registration.vue';


export default {
    components: { Questions, Registration }
}

</script>