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

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.prodCard {
    width: calc(100% / 6);
    aspect-ratio: 3 / 4;
    padding: 10px;
    font-size: 12px;
    cursor: pointer;

    &:hover {
        background-color: #313131;
    }

    img {
        width: 100%;
        aspect-ratio: 1 / 1;
        object-fit: cover;
        object-position: top;
        margin-bottom: 10px;
    }

}
</style>
