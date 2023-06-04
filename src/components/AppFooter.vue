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
                            url: "#"
                        }, {
                            text: "Comics",
                            url: "#"
                        }, {
                            text: "Movies",
                            url: "#"
                        }, {
                            text: "TV",
                            url: "#"
                        }, {
                            text: "Games",
                            url: "#"
                        }, {
                            text: "Videos",
                            url: "#"
                        }, {
                            text: "News",
                            url: "#"
                        }
                    ]
                }, {
                    title: 'SHOP',
                    links: [
                        {
                            text: "Shop DC",
                            url: "#"
                        }, {
                            text: "Shop DC Collectibles",
                            url: "#"
                        }
                    ]
                }, {
                    title: 'DC',
                    links: [
                        {
                            text: "Terms Of Use",
                            url: "#"
                        }, {
                            text: "Privacy policy (New)",
                            url: "#"
                        }, {
                            text: "Ad Choices",
                            url: "#"
                        }, {
                            text: "Advertising",
                            url: "#"
                        }, {
                            text: "Jobs",
                            url: "#"
                        }, {
                            text: "Subscription",
                            url: "#"
                        }, {
                            text: "Talent Workshops",
                            url: "#"
                        }, {
                            text: "CPSC Certificates",
                            url: "#"
                        }, {
                            text: "Ratings",
                            url: "#"
                        }, {
                            text: "Shop Help",
                            url: "#"
                        }, {
                            text: "Contact Us",
                            url: "#"
                        }
                    ]
                }, {
                    title: 'SITES',
                    links: [
                        {
                            text: "DC",
                            url: "#"
                        }, {
                            text: "MAD Magazine",
                            url: "#"
                        }, {
                            text: "DC Kids",
                            url: "#"
                        }, {
                            text: "DC Universe",
                            url: "#"
                        }, {
                            text: "DC Power VIsa",
                            url: "#"
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
        <!-- Top Footer -->
        <div id="footTop">
            <div class="container">
                <!-- Nav Menu -->
                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="textImage">DIGITAL COMICS</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <div class="textImage">DC MERCHANDISE</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div class="textImage">SUBSCRIBTION</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div class="textImage">COMIC SHOP LOCATOR</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div class="textImage">DC POWER VISA</div>
                </a>
            </div>
        </div>

        <!-- Main Footer -->
        <div id="footMain">
            <div class="container">
                <nav>
                    <!-- Nav Column -->
                    <div class="navCol">
                        <h2>DC COMICS</h2>
                        <ul>
                            <li v-for="(link, idx) in footerLinks[0].links" :key="idx">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>

                        <h2>SHOP</h2>
                        <ul>
                            <li v-for="(link, idx) in footerLinks[1].links" :key="idx">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>

                    <!-- Nav Column -->
                    <div class="navCol">
                        <h2>DC</h2>
                        <ul>
                            <li v-for="(link, idx) in footerLinks[2].links" :key="idx">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>

                    <!-- Nav Column -->
                    <div class="navCol">
                        <h2>SITES</h2>
                        <ul>
                            <li v-for="(link, idx) in footerLinks[3].links" :key="idx">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </nav>
            </div>
        </div>

        <!-- Bottom Footer -->
        <div id="footBottom">
            <div class="container">
                <button>SIGN-UP NOW!</button>
                <!-- social media -->
                <div class="socialMedia">
                    <span>
                        <a href="#">FOLLOW US</a>
                    </span>
                    <ul>
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
@use '../styles/partials/variables.scss' as *;

footer {
    font-size: 0.7em;
}

#footTop {
    height: 100px;
    background-color: #0678db;
    color: #ffffff;

    .container {
        justify-content: space-evenly;
        gap: 10px;
    }
}

.sectionLink {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 60%;
    padding: 10px;
    border-radius: 10px;

    &:hover {
        background-color: #0f68b7;
    }

    .sectionImage {
        width: 40px;
        height: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .textImage {
        margin-left: 10px;
    }
}

#footMain {
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

            .navCol {
                min-width: 120px;
                padding: 10px;
                margin: 10px;

                h2 {
                    font-size: 1.2em;
                    margin: 10px 0;
                }

                li {
                    padding: 3px;
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
    height: 75px;
    background-color: #303030;

    .container {
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
            color: #0c7cec;
            align-items: center;

            span a:hover {
                font-size: 1.1em;
                font-weight: 700;
            }

            ul {
                display: flex;
                gap: 10px;
                color: #787878;

                li {
                    width: 20px;

                    img {
                        border-radius: 50%;
                    }

                    img:hover {
                        background-color: #bbbbbb;
                    }
                }
            }
        }
    }
}

//DEBUG
</style>