<script>
import CardDefault from './CardDefault.vue';
import AppMainJumbo from './AppMainJumbo.vue';

export default {
    components: {
        CardDefault,
        AppMainJumbo
    },
    data() {
        return {
            cardList: [
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <AppMainJumbo />
    <section>
        <div class="container">
            <h2>CURRENT SERIES</h2>
            <CardDefault
            v-for="element in cardList" 
            :img="element.thumb"
            :text="element.series"/>
        </div>
        <div class="button">
            <a href="#">LOAD MORE</a>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #000;
    color: #fff;

    h2{
        position: absolute;
        padding: 10px 20px;
        background-color: #3050D9;
        top: -60px;
        left: 0;
    }

    .container {
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        position: relative;
    }

    :deep(.foto){
        width: 100%;
        margin-bottom: 5px;
        img{
            max-width: 100%;
            aspect-ratio: 1/1;
            object-fit: cover;
        }
    }
    :deep(span){
        text-transform: uppercase;

    }
}
.button{
    max-width: 200px;
    margin: 0 auto;
    padding-top: 20px;
}
a{
    background-color: #3050D9;
    padding: 10px 40px;
    color: #fff;
}
</style>