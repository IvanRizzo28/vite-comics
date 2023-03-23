<script>
import AppFooterJumbo from "./AppFooterJumbo.vue";
import AppFooterInformation from "./AppFooterInformation.vue";

export default{
    components:{
        AppFooterJumbo,
        AppFooterInformation
    }
}
</script>

<template>
    <footer>
        <div class="jumbo">
            <div class="container">
                <AppFooterJumbo />
                <img src="/dc-logo-bg.png" alt="">
            </div>
        </div>
        <div class="container">
            <AppFooterInformation />
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    @mixin conteainer-Flex{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    footer{
        background-color: #303030;
        .jumbo{
            background-image: url("./../assets/footer-bg.jpg");
            background-size: cover;
        }
        .container{
            padding: 20px 0;
            max-width: 1200px;
            margin: 0 auto;
            position: relative;
            @include conteainer-Flex;
            overflow: hidden;
            img{
                position: absolute;
                right: 0;
                top: 50%;
                transform: translateY(-50%);
            }
        }
    }
</style>