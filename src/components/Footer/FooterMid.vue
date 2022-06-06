<template>
    <section class="footer-mid">
        <div class="container">
            <div class="col-sx">
                <div class="col">
                    <div v-for="(link,index) in colOne" :key="index">
                        <h3>{{link.title}}</h3>
                        <nav>
                            <ul class="footers-links">
                                <li v-for="(link,index) in link.singleLink" :key="index"><a href=""><small>{{link.text}}</small></a></li>
                            </ul>
                        </nav>
                    </div>
                </div>
                <div class="col">
                    <div v-for="(link,index) in colTwo" :key="index">
                        <h3>{{link.title}}</h3>
                        <nav>
                            <ul class="footers-links">
                                <li v-for="(link,index) in link.singleLink" :key="index"><a href=""><small>{{link.text}}</small></a></li>
                            </ul>
                        </nav>
                    </div>
                </div>
                <div class="col">
                    <div v-for="(link,index) in colThree" :key="index">
                        <h3>{{link.title}}</h3>
                        <nav>
                            <ul class="footers-links">
                                <li v-for="(link,index) in link.singleLink" :key="index"><a href=""><small>{{link.text}}</small></a></li>
                            </ul>
                        </nav>
                    </div>
                </div>
            </div>
            <div class="col-dx"></div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterMid',
    data(){
        return {
            colOne: [
                {
                    title: 'Dc comics',
                    singleLink: [
                        {
                            text: 'Characters',
                            url: '#'
                        },
                        {
                            text: 'Comics',
                            url: '#'
                        },
                        {
                            text: 'Movies',
                            url: '#'
                        },
                        {
                            text: 'TV',
                            url: '#'
                        },
                        {
                            text: 'Games',
                            url: '#'
                        },
                        {
                            text: 'Videos',
                            url: '#'
                        },
                        {
                            text: 'News',
                            url: '#'
                        },
                    ]
                },
                {
                    title: 'Shop',
                    singleLink: [
                        {
                            text: 'Shop DC',
                            url: '#'
                        },
                        {
                            text: 'Shop DC Collectibles',
                            url: '#'
                        },
                    ]   
                }

            ],
            colTwo:[
                {
                    title: 'Dc',
                    singleLink: [
                        {
                            text: 'Terms Of Use',
                            url: '#'
                        },
                        {
                            text: 'Privacy policy (New)',
                            url: '#'
                        },
                        {
                            text: 'Ad Choices',
                            url: '#'
                        },
                        {
                            text: 'Advertising',
                            url: '#'
                        },
                        {
                            text: 'Jobs',
                            url: '#'
                        },
                        {
                            text: 'Subscriptions',
                            url: '#'
                        },
                        {
                            text: 'Talent Workshops',
                            url: '#'
                        },
                        {
                            text: 'CPSC Certificates',
                            url: '#'
                        },
                        {
                            text: 'Ratings',
                            url: '#'
                        },
                        {
                            text: 'Shop Help',
                            url: '#'
                        },
                        {
                            text: 'Contact Us',
                            url: '#'
                        },
                    ]
                }
            ],
            colThree: [
                {
                    title: 'Sites',
                    singleLink: [
                        {
                            text: 'DC',
                            url: '#'
                        },
                        {
                            text: 'MAD Magazine',
                            url: '#'
                        },
                        {
                            text: 'DC Kids',
                            url: '#'
                        },
                        {
                            text: 'DC Universe',
                            url: '#'
                        },
                        {
                            text: 'DC Power Visa',
                            url: '#'
                        }
                    ]
                }
            ]    
        }
    }
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