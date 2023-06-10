<template>
    <div class="materials-card overflow-hidden rounded-lg w-[340px] h-[230px] lg:h-[530px] flex items-end justify-start p-[25px] lg:p-[40px]"
        :style="`background-image: url(${data.image})`">
        <div class="text">
            <p class="text-white relative font-bold text-2xl lg:text-[40px] leading-[1.3]">{{ data.name }}</p>
        </div>

    </div>
</template>

<script>

export default {
    props: {
        data: {
            type: Object,
            require: true
        }
    }

}

</script>


<style lang="scss" scoped>
.materials-card {
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    cursor: pointer;
    transition: transform 0.3s;
    position: relative;

    &::before{
        content: '';
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(180deg, rgba(49, 24, 10, 0) 0%, rgba(15, 12, 46, 0.03375) 6.25%, rgba(10, 12, 49, 0.54) 100%);
    }

    &:hover {
        transform: translateY(-30px);
    }
}
</style>