<template>
    <header class="header z-50 fixed top-0 w-full transition-all lg:pt-8" :class="isScrolled ? 'header-scrolled lg:pt-0' : 'lg:pt-8'">
        <div class="container flex items-center">
            <HeaderLogo></HeaderLogo>
            <HeaderMenu></HeaderMenu>
            <HeaderActions @openMenu="toggleMenu" :scrolled="isScrolled"></HeaderActions>
        </div>
    </header>
    <Transition name="menu">
        <HiddenMenu class="z-50" v-if="isOpen" @closeMenu="toggleMenu"></HiddenMenu>
    </Transition>
</template>

<script>
import { onMounted } from 'vue';
import HeaderActions from './components/HeaderActions.vue';
import HeaderLogo from './components/HeaderLogo.vue';
import HeaderMenu from './components/HeaderMenu.vue';
import HiddenMenu from './components/HiddenMenu.vue';


export default {
    components: { HeaderLogo, HeaderMenu, HeaderActions, HiddenMenu },
    data() {
        return {
            isOpen: false,
            isScrolled: false,
        }
    },
    methods: {
        toggleMenu() {
            this.isOpen = !this.isOpen
        },
    },
    mounted() {
        window.addEventListener('scroll', () => {
            if(window.scrollY) {
                this.isScrolled = true
            } else {
                this.isScrolled = false
            }
        })

    }

}
</script>

<style>
.menu-enter-active,
.menu-leave-active {
    transition: 0.5s ease;
}

.menu-enter-from,
.menu-leave-to {
    transform: translateX(100%);
}


.header-scrolled {
    background: rgba(255, 255, 255, 0.7);
    backdrop-filter: blur(5px);
}
</style>