<template>
    <footer class="footer bg-gray text-white pt-3 pb-5 lg:py-6">
        <div class="container flex gap-y-5 justify-between items-center flex-wrap">
            <FooterLogo class="order-1" />
            <FooterCopyright class="order-5" />
            <FooterLinks class="order-2" />
            <FooterNav class="order-3" />
            <FooterActions class="order-4" />
        </div>
    </footer>
    

</template>

<script>
import FooterActions from './components/FooterActions.vue';
import FooterCopyright from './components/FooterCopyright.vue';
import FooterLinks from './components/FooterLinks.vue';
import FooterLogo from './components/FooterLogo.vue';
import FooterNav from './components/FooterNav.vue';

export default {
    components: { FooterLogo, FooterCopyright, FooterLinks, FooterNav, FooterActions }
}
</script>