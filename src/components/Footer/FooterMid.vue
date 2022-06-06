<template>
    <section class="footer-mid">
        <div class="container">
            <div class="col-sx">
                <div class="col">
                    <h3>Dc Comics</h3>
                    <nav>
                        <ul class="footers-links">
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                        </ul>
                    </nav>
                    <h3>Shop</h3>
                    <nav>
                        <ul class="footers-links">
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                        </ul>
                    </nav>
                </div>
                <div class="col">
                    <h3>Dc</h3>
                    <nav>
                        <ul class="footers-links">
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                        </ul>
                    </nav>
                </div>
                <div class="col">
                    <h3>Sites</h3>
                    <nav>
                        <ul class="footers-links">
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                            <li><a href=""><small>link</small></a></li>
                        </ul>
                    </nav>
                </div>
            </div>
            <div class="col-dx"></div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterMid'
}
</script>

<style lang="scss">

.footer-mid{
    background-image: var(--footer-mid-bg-img);
    background-repeat: no-repeat;
    background-size: cover;

    & .container{
        display: flex;
    }

    & .col-sx{
        padding: 2.5rem 0;
        width: 50%;
        display: flex;

        & .col{
            width: calc(100% / 3);
        }

        & h3{
            margin: .9375rem 0;
            color: #fff;
            text-transform: uppercase;
        }

        & .footers-links{
            list-style: none;
            & a{
                text-decoration: none;
                color: var(--text-lightgrey);
            }
        }
    }

    & .col-dx{
        background-image: var(--footer-mid-bg-logo);
        background-position: center;
        background-repeat: no-repeat;
        width: 50%;
        height: 400px;
        z-index: 10;
    }
}

</style>