<script>
    import AppHeader from './components/AppHeader.vue';
    import AppMain from './components/AppMain.vue';
    import AppFooter from './components/AppFooter.vue';

    export default {
        components: {
            AppHeader,
            AppMain,
            AppFooter
        }
    }
</script>

<template>
    <div>
        <AppHeader />
        <AppMain />
        <AppFooter />
    </div>
</template>

<style lang="scss">
    @use './styles/general.scss' as *;
    @use './styles/partials/mixins' as *;
    @use './styles/partials/variables';
</style>