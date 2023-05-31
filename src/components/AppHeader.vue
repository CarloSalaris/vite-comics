<script>

export default {
    name: "AppHeader",
}



</script>

<template>
    <header>
        <div class="container">
            <!-- Logo -->
            <div id="headerLogo">
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="">
                </a>
            </div>
            <!-- Nav Menu -->
            <nav>
                <ul>
                    <li><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                    <li class="active"><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                    <li><a href="#">element</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.container {
    justify-content: space-between;
}

#headerLogo {
    height: 75px;
    padding: 15px 0;
}

a {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
}

ul {
    display: flex;
    gap: 10px;
    height: 100%;

    li.active,
    li:hover {
        color: #0678db;
    }

    li.active {
        border-bottom: 4px solid #0678db;
    }

}

//DEBUG
header {
    border-bottom: dotted 1px black;
}
</style>
