<script>
import ProductCard from './ProductCard.vue'

export default {
    name: "ProductList",
    components: {
        ProductCard
    }
}

</script>

<template>
    <section class="prodList">
        <ProductCard />
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.prodList {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
}
</style>
