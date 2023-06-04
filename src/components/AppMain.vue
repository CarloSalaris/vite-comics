<script>

import ProductList from './ProductList.vue';

export default {
    name: "AppMain",
    components: {
        ProductList
    }
}



</script>

<template>
    <main>
        <div class="container">
            <!-- cards container -->
            <ProductList />

            <div class="buttons">
                <button>LOAD MORE</button>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

main {
    background-color: #1c1c1c;
    color: #ffffff;
    min-height: 75px;
    padding: 15px 0;
}

.container {
    display: block;
}

.buttons {
    text-align: center;

    button {
        padding: 10px 50px;
        color: #ffffff;
        font-weight: 600;
        background-color: #0282f9;
        border: none;
        cursor: pointer;
    }

    button:hover {
        color: #0282f9;
        background-color: #91caff;
    }
}
</style>
