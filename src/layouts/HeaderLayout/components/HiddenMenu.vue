<template>
    <div class="hidden-menu bg-white fixed left-0 top-0 w-full h-full p-5 flex flex-col justify-between">
        <div class="wrapper">
            <div class="head flex justify-between items-center">
                <HeaderLogo></HeaderLogo>

                <button class="close-btn w-7 h-7 flex justify-center items-center" @click="$emit('closeMenu')">
                    <img src="@/assets/icons/times.svg" alt="times-icon">
                </button>
            </div>
            <div class="menu-list">
                <ul class="menu">
                    <li class="mt-12 text-dark text-xl" v-for="item in menuItems" :key="item">
                        {{ item.name }}
                    </li>
                </ul>
            </div>
            <div class="action mt-16">
                <TheButton>Заказать звонок</TheButton>
            </div>
        </div>
        <div class="copyright">
            <p class="text-xs text-center text-[#646464]">
                Политика конфиденциальности © спец-транс, 2023
            </p>
        </div>
    </div>
</template>


<script>
import TheButton from '../../../ui/TheButton.vue';
import menuList from '../menuList';
import HeaderLogo from './HeaderLogo.vue';

 

export default {
    components: { HeaderLogo, TheButton },
    data() {
        return {
            menuItems: menuList,
        }
    }

}


</script>