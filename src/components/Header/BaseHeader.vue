<template>
  <header class="header">
        <div class="container">
            <div class="header__logo">
                <img src="../../assets/img/dc-logo.png" alt="Dc logo">
            </div>
            <nav class="header__navbar">
                <ul class="header__list">
                    <li><a href="#">characters</a></li>
                    <li><a href="#">comics</a></li>
                    <li><a href="#">movies</a></li>
                    <li><a href="#">tv</a></li>
                    <li><a href="#">games</a></li>
                    <li><a href="#">collectibles</a></li>
                    <li><a href="#">videos</a></li>
                    <li><a href="#">fans</a></li>
                    <li><a href="#">news</a></li>
                    <li><a href="#">shop</a></li>
                </ul>
            </nav>
        </div>
  </header>
</template>

<script>
export default {
    name: 'BaseHeader'
}
</script>

<style lang="scss">
.header{
    
    & .container{
        height: 6.25rem;
    }

    & .container, &__list{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }  
    
    &__navbar{
        ul{
            list-style: none;
            gap: 1.25rem;
            text-transform: uppercase;
        }

        li{
            display: inline-block;
        }

        a{
            text-decoration: none;
            display: inline-block;
            color: var(--text-darkgrey);
            font-weight: bold;
        }

        .active a{
            color: var(--primary-color);
        }
    }

    &__logo img{
        width: 5rem;
    }
}
</style>