<script>

export default {
    name: "ProductCard",
    props: {
        details: Object,
    }
}

</script>

<template>
    <!-- Blocco prodotto -->
    <div class="prodCard">
        <img :src="details.thumb" :alt="details.series" loading="lazy">
        <h3>{{ details.series }}</h3>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;

.prodCard {
    width: calc(100% / 6);
    border: 1px dotted #ffffff;
    padding: 10px;

    img {
        width: 100%;
        aspect-ratio: 1 / 1;
        object-fit: cover;
        object-position: top;
    }

}
</style>
