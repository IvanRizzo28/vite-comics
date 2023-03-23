<script>
</script>

<template>
    <a href="#" class="btn">SIGN-UP NOW</a>
    <div>
        <span>FOLLOW US</span>
        <img src="../assets/footer-facebook.png" alt="">
        <img src="../assets/footer-youtube.png" alt="">
        <img src="../assets/footer-periscope.png" alt="">
        <img src="../assets/footer-twitter.png" alt="">
        <img src="../assets/footer-pinterest.png" alt="">
    </div>
</template>

<style lang="scss" scoped>
    a{
        color: #fff;
        padding: 10px 20px;
        border: 1px solid #3050D9;
    }
    div{
        display: flex;
        align-items: center;
        &>*{
            margin-left: 10px
        }
        span{
            margin-right: 10px;
            font-weight: bold;
            font-size: 18px;
            color: #3050D9;
        }
    }
</style>