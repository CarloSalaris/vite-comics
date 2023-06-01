<script>

export default {
    name: "AppFooter",

    data() {
        return {
            //dati
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
                    <div class="textImage">text</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <div class="textImage">text</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div class="textImage">text</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div class="textImage">text</div>
                </a>

                <a href="#" class="sectionLink">
                    <div class="sectionImage">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div class="textImage">text</div>
                </a>
            </div>
        </div>

        <!-- Main Footer -->
        <div id="footMain">
            <div class="container">
                <nav>
                    contenuto nav
                </nav>
            </div>
        </div>

        <!-- Bottom Footer -->
        <div id="footBottom">
            <div class="container">
                <button>SIGN-UP NOW!</button>
                <!-- social media -->
                <div class="socialMedia">
                    <span class="followUs">
                        <a href="#">FOLLOW US</a>
                    </span>
                    <ul>
                        <li>
                            <a href="#">
                                <i class="fa-brands fa-facebook"></i>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <i class="fa-brands fa-twitter"></i>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <i class="fa-brands fa-youtube"></i>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <i class="fa-brands fa-pinterest"></i>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <i class="fa-solid fa-location-dot"></i>
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
    height: 250px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;

    .container {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;
        background-size: 380px;

        nav {
            color: #ffffff;
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

        .socialMedia {
            display: flex;
            gap: 10px;
            color: #0c7cec;

            ul {
                display: flex;
                gap: 10px;
                color: #787878;
            }
        }
    }
}

//DEBUG
</style>