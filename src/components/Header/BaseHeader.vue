<template>
  <header class="header">
        <div class="container">
            <div class="header__logo">
                <img src="../../assets/img/dc-logo.png" alt="Dc logo">
            </div>
            <nav class="header__navbar">
                <ul class="header__list">
                    <li v-for="(link,index) in links" :key="index" :class="{active: link.current}"><a href="#" @click="clicked(link)">{{link.text}}</a></li>
                </ul>
            </nav>
        </div>
  </header>
</template>

<script>
export default {
    name: 'BaseHeader',
    data(){
        return {
            links: [
                {
                   text: 'characters',
                   url: '#',
                   current: false
                },
                {
                   text: 'comics',
                   url: '#',
                   current: false
                },
                {
                   text: 'movies',
                   url: '#',
                   current: false
                },
                {
                   text: 'tv',
                   url: '#',
                   current: false
                },
                {
                   text: 'games',
                   url: '#',
                   current: false
                },
                {
                   text: 'collectibles',
                   url: '#',
                   current: false
                },
                {
                   text: 'videos',
                   url: '#',
                   current: false
                },
                {
                   text: 'fans',
                   url: '#',
                   current: false
                },
                {
                   text: 'news',
                   url: '#',
                   current: false
                },
                {
                   text: 'shop',
                   url: '#',
                   current: false
                },
            ]
        }
    },
    methods: {
        clicked(link){
            console.log(link)
           if(!link.current == true){
               link.current = true;
           }else{
               link.current = false
           }
        }
    }
}
</script>

<style lang="scss">
@import '../../assets/style/mixins.scss';

.header{
    height: 100%;
    &__list{
        height: 100%;
        display: flex;
        align-items: center;
        height: 100%;
        
    }

    & .container{
        height: 6.25rem;
    }

    & .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }  
    
    &__navbar{
        height: 100%;
        ul{
            @include listStyle;
            gap: 1.25rem;
            text-transform: uppercase;
            height: 100%;
        }

        li{
            height: 100%;
            line-height: 100px;
        }

        a{
            text-decoration: none;
            display: inline-block;
            color: var(--text-darkgrey);
            font-weight: bold;
            border-bottom: 5px solid transparent;
            height: 100%;

            &:hover{
                color: var(--primary-color);
            }
        }

        .active a{
            color: var(--primary-color);
            border-bottom: 5px solid var(--primary-color);
        }


    }

    &__logo img{
        width: 5rem;
    }
}
</style>