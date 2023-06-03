<template>
    <header class="header fixed top-0 w-full">
        <div class="container flex items-center">
            <HeaderLogo></HeaderLogo>
            <HeaderMenu></HeaderMenu>
            <HeaderActions @openMenu="toggleMenu"></HeaderActions>
            <Transition name="menu">
                <HiddenMenu v-if="isOpen" @closeMenu="toggleMenu"></HiddenMenu>
            </Transition>
        </div>
    </header>
</template>

<script>
import HeaderActions from './components/HeaderActions.vue';
import HeaderLogo from './components/HeaderLogo.vue';
import HeaderMenu from './components/HeaderMenu.vue';
import HiddenMenu from './components/HiddenMenu.vue';


export default {
    components: { HeaderLogo, HeaderMenu, HeaderActions, HiddenMenu },
    data() {
        return {
            isOpen: false
        }
    },
    methods: {
        toggleMenu() {
            this.isOpen = !this.isOpen
        }
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
</style>