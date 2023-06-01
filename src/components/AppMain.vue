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
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

main {
    background-color: black;
    color: #ffffff;
    min-height: 75px;
    padding: 15px 0;
}
</style>
