<script>
import ProductCard from './ProductCard.vue'

export default {
    name: "ProductList",
    components: {
        ProductCard
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1tpin068isbn_0.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BTMA017_0.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i0.wp.com/batman-news.com/wp-content/uploads/2021/08/Batman-Superman-2021-Annual-1.jpg?fit=780%2C1200&quality=80&strip=info&ssl=1",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/I/41nGyVF7C2L.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ebayimg.com/images/g/9CsAAOSwLfpfQY8h/s-l1600.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/I/51sZeblq1fL.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://mycomics.it/wp-content/uploads/sites/16/2022/12/FUMCAWOPA0008.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}

</script>

<template>
    <section class="prodList">
        <!-- Etichetta "Current Series" -->
        <div class="infoTab">
            <h2>CURRENT SERIES</h2>
        </div>

        <!-- Blocco prodotto -->
        <ProductCard v-for="(comic, idx) in comics" :key="idx" :details="comic" />
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.prodList {
    position: relative;
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    margin: 20px 0;
}

.infoTab {
    position: absolute;
    top: - 65px;
    left: 0;
    background-color: #0282f9;
    padding: 10px 20px;
}
</style>
