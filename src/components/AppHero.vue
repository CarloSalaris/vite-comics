<script>

export default {
    name: "AppHero",

}

</script>

<template>
    <div id="hero"></div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

#hero {
    height: 250px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
}
</style>
