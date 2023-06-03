<template>
    <div class="header-actions ml-auto">
        <TheButton class="hidden lg:block" v-if="true">Заказать звонок</TheButton>

        <button class="burger-btn w-5 h-5 flex justify-center items-center lg:hidden" @click="$emit('openMenu')">
            <img src="@/assets/icons/burger.svg" alt="burger-icon">
        </button>
    </div>
</template>

<script>
import TheButton from '../../../ui/TheButton.vue'

export default {
    components: {TheButton}
}

</script>