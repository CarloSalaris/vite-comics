<script>

export default {
    name: "AppFooter",
}



</script>

<template>
    <footer>
        <!-- Top Footer -->
        <div id="FootTop">
            <div class="container">
                <!-- Nav Menu -->
                <nav>
                    <ul>
                        <li><a href="#">
                                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                                <div class="textImage">text</div>
                            </a></li>
                        <li><a href="#">
                                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                                <div class="textImage">text</div>
                            </a></li>
                        <li><a href="#">
                                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                                <div class="textImage">text</div>
                            </a></li>
                        <li><a href="#">
                                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                                <div class="textImage">text</div>
                            </a></li>
                        <li><a href="#">
                                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                                <div class="textImage">text</div>
                            </a></li>
                    </ul>
                </nav>
            </div>
        </div>

        <!-- Main Footer -->
        <div></div>

        <!-- Bottom Footer -->
        <div></div>


    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

#FootTop {
    height: 100px;
    background-color: #0678db;
    color: #ffffff;
}

.container {
    height: 100%;
}

.textImage {
    margin-left: 10px;
}

nav {
    height: 100%;
    width: 100%;
    padding: 30px;
}

a {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
}

ul {
    display: flex;
    justify-content: space-evenly;
    gap: 10px;
    height: 100%;

    // li.active,
    // li:hover {
    //     color: #0678db;
    //     background-color: #ffffff;
    // }
}

//DEBUG
</style>