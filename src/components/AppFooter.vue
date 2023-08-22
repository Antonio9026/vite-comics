<script>
export default {
    name: "AppFooter",

    data() {
        return {
            footerLinks: [
                {
                    title: 'DC COMICS',
                    links: [
                        {
                            text: "Characters",
                        }, {
                            text: "Comics",
                        }, {
                            text: "Movies",
                        }, {
                            text: "TV",

                        }, {
                            text: "Games",

                        }, {
                            text: "Videos",

                        }, {
                            text: "News",

                        }
                    ]
                }, {
                    title: 'SHOP',
                    links: [
                        {
                            text: "Shop DC",

                        }, {
                            text: "Shop DC Collectibles",

                        }
                    ]
                }, {
                    title: 'DC',
                    links: [
                        {
                            text: "Terms Of Use",

                        }, {
                            text: "Privacy policy (New)",

                        }, {
                            text: "Ad Choices",

                        }, {
                            text: "Advertising",

                        }, {
                            text: "Jobs",

                        }, {
                            text: "Subscription",

                        }, {
                            text: "Talent Workshops",

                        }, {
                            text: "CPSC Certificates",

                        }, {
                            text: "Ratings",

                        }, {
                            text: "Shop Help",

                        }, {
                            text: "Contact Us",

                        }
                    ]
                }, {
                    title: 'SITES',
                    links: [
                        {
                            text: "DC",

                        }, {
                            text: "MAD Magazine",

                        }, {
                            text: "DC Kids",

                        }, {
                            text: "DC Universe",

                        }, {
                            text: "DC Power VIsa",

                        }
                    ]
                }
            ]
        }
    }
}



</script>


<template>
    <footer>
        <div class="footer-main">
            <div class="container">
                <nav>
                    <div class="nav-col">
                        <h2>DC COMICS</h2>
                        <ul>
                            <li v-for="(link, i) in footerLinks[0].links"><a href="#">{{ link.text }}</a></li>
                        </ul>

                        <h2>SHOP</h2>
                        <ul>
                            <li v-for="(link, i) in footerLinks[1].links"><a href="">{{ link.text }}</a></li>
                        </ul>
                    </div>
                    <div class="nav-col">
                        <h2>DC</h2>
                        <ul>
                            <li v-for="(link, i) in footerLinks[2].links"><a href="">{{ link.text }}</a></li>
                        </ul>
                    </div>
                    <div class="nav-col">
                        <h2>SITES</h2>
                        <ul>
                            <li v-for="(link, i) in footerLinks[3].links"><a href=""></a>{{ link.text }}</li>
                        </ul>
                    </div>
                </nav>
            </div>
        </div>
        <div id="footBottom">
            <div class="foot-bottom-container">
                <button>SIGN-UP NOW!</button>
                <!-- social media -->
                <div class="socialMedia">
                    <span>
                        <a href="#">FOLLOW US</a>
                    </span>
                    <ul class="foot-bottom-list">
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png" alt="">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
.footer-main {
    min-height: 250px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;

    .container {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;
        background-size: 380px;

        nav {
            color: #ffffff;
            display: flex;

            .nav-col {
                min-width: 120px;
                padding: 10px;
                margin: 10px;

                h2 {
                    font-size: 13px;
                    margin: 10px 0;
                }

                li {
                    padding: 3px;
                    font-size: 12px;
                    color: #687980;

                    a {
                        color: #687980;
                    }
                }

                li:hover {
                    color: #cecece;
                    text-decoration: underline;
                }
            }
        }
    }
}










#footBottom {
    height: 70px;
    background-color: #303030;

    .foot-bottom-container {
        width: 70%;
        margin: 0 auto;
        height: 100%;
        max-width: 1170px;
        display: flex;
        align-items: center;
        justify-content: space-between;

        button {
            color: #ffffff;
            background-color: inherit;
            border: solid 1px #0c7cec;
            padding: 10px;
            cursor: pointer;
        }

        button:hover {
            border: solid 2px #0c7cec;
            color: #cecece;

        }

        .socialMedia {
            display: flex;
            gap: 10px;
            align-items: center;

            .foot-bottom-list {

                display: flex;
                gap: 10px;
                color: #787878;

                img {
                    border-radius: 50%;
                }

                img:hover {
                    background-color: #bbbbbb;
                }
            }

            span a {
                color: #0c7cec;
            }

            span a:hover {
                font-size: 1.1em;
                font-weight: 700;
            }

        }
    }
}
</style>