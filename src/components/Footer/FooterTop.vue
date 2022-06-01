<template>
    <section class="footer-top">
        <div class="container">
            <ul class="merch-list">
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-digital-comics.png" alt="Digital comics image">
                        <span>Digital comics</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-merchandise.png" alt="Merchandise image">
                        <span>Dc merchandise</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-subscriptions.png" alt="Subscription image">
                        <span>Subscription</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-shop-locator.png" alt="Shop locator image">
                        <span>Comic shop locator</span>
                    </a>
                </li><li>
                    <a href="#">
                        <img class="svg" src="../../assets/img/buy-dc-power-visa.svg" alt="Power visa image">
                        <span>Dc power visa</span>
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterTop'
}
</script>

<style lang="scss">

    @import '../../assets/style/mixins.scss';
    .footer-top{
        background-color: var(--primary-color);
        padding: 30px 0;
    }

    .merch-list{
        @include listStyle;
        display: flex;
        align-items: center;
        justify-content: space-between;

        & a {
            text-decoration: none;
            color: #fff;
            display: flex;
            align-items: center;
            gap: .625rem;
            text-transform: uppercase;
        }

        & img{
            height: 3.75rem;

            &.svg{
                height: 2.5rem;
            }
        }
    }
</style>