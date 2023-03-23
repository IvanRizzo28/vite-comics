<script>
    export default{
        data(){
            return {
                active: 1,
                menuList: [
                    {
                        nome: 'Characters',
                        link: '#'
                    },
                    {
                        nome: 'Comics',
                        link: '#'
                    },
                    {
                        nome: 'Movies',
                        link: '#'
                    },
                    {
                        nome: 'Tv',
                        link: '#'
                    },
                    {
                        nome: 'games',
                        link: '#'
                    },
                    {
                        nome: 'collectibles',
                        link: '#'
                    },
                    {
                        nome: 'videos',
                        link: '#'
                    },
                    {
                        nome: 'fans',
                        link: '#'
                    },
                    {
                        nome: 'news',
                        link: '#'
                    },
                    {
                        nome: 'shop',
                        link: '#'
                    },
                ]
            }
        },
        methods:{
            isActive(i){
                if (i===this.active) return 'active';
                return '';
            }
        }
    }
</script>

<template>
    <nav>
        <ul>
            <li v-for="(element,index) in menuList">
                <a :href="element.link" :class="isActive(index)">{{ element.nome }}</a>
            </li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
    ul{
        list-style: none;
        display: flex;

        li{
          a{
            display: inline-block;
            padding: 15px;
            text-decoration: none;
            text-transform: uppercase;
            color: #000;
          }  
        }
    }

    .active{
        border-bottom: 5px solid #3050D9;
    }
</style>