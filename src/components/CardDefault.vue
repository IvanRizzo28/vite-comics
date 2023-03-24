<script>
export default {
    name: 'Card',
    props: {
        img: String,
        text: String
    }
}
</script>

<template>
    <div class="card">
        <div class="content">
            <div class="foto">
                <img :src="img" :alt="text">
            </div>
            <span>{{ text }}</span>
        </div>
    </div>
</template>

<style scoped lang="scss">
.card {
    width: calc(100% / 6);
    padding: 20px;
}
</style>