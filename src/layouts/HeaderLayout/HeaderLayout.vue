<template>
    <header class="header fixed top-0 w-full">
        <div class="container flex items-center">
            <HeaderLogo></HeaderLogo>
            <HeaderMenu></HeaderMenu>
            <HeaderActions></HeaderActions>
        </div>
    </header>
    

</template>

<script>
import HeaderActions from './components/HeaderActions.vue';
import HeaderLogo from './components/HeaderLogo.vue';
import HeaderMenu from './components/HeaderMenu.vue';


export default {
    components: { HeaderLogo, HeaderMenu, HeaderActions }
}
</script>