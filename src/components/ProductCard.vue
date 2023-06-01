<script>

export default {
    name: "ProductCard",
}

</script>

<template>
    <!-- Blocco prodotto -->
    <div class="prodCard">
        <img src="../assets/img/dc-logo.png" alt="">
        <h3>testo immagine</h3>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.prodCard {
    width: calc(100% / 6);
    border: 1px dotted #ffffff;

}
</style>
