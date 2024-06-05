<template>
    <v-app>
        <AppHearder />
        <AppBody />
        <!-- <TheHeader />
        <TheIntro />
        <TheNewArrivals />
        <TheTopSelling />
        <TheItemCategory />
        <TheFeetback /> -->
        <AppFooter />
        <!-- <div style="height: 500px"></div> -->
    </v-app>
</template>

<script>
import AppHearder from './components/layouts/AppHeader.vue';
import AppBody from './components/layouts/AppBody.vue';
import AppFooter from './components/layouts/AppFooter.vue';
export default {
    components: { AppHearder, AppBody, AppFooter },
    data() {
        return {};
    },
};
</script>

<style lang="scss" scoped>
@import './assets/styles/global.scss';
</style>
