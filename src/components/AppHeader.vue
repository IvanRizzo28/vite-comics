<script>
    import AppMenu from './AppMenu.vue';

    export default{
        components:{
            AppMenu
        }
    }
</script>

<template>
    <header>
        <img src="/dc-logo.png" alt="Logo">
        <AppMenu />
    </header>
</template>

<style lang="scss" scoped>
    @mixin conteainer-Flex{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    header{
        padding: 20px 0;
        max-width: 1200px;
        margin: 0 auto;
        @include conteainer-Flex;
    }

    img{
        width: 80px;
    }
</style>