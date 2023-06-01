<script >
import { createDOMCompilerError } from '@vue/compiler-dom';
import AppCard from './AppCard.vue';
import AppJumbotron from './AppJumbotron.vue';

export default {
    components: {
        AppCard, AppJumbotron
    },
    name: "AppMain",
    data() {
        return {
            cards: [
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
                    "thumb": "../../public/img/Batman_Beyond.webp",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/img/Batman_Superman.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/img/Batman_Superman_Annual.webp",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/img/Batman_The_Joker_War_Zone.webp",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/img/Batman_Three_Jokers_Collected.webp",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/img/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.webp",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/img/Catwoman_Vol_2_1.webp",
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
    <main>
        <AppJumbotron />
        <div class="title-container">
            <div class="title">CURRENT SERIES</div>
        </div>
        <div class="container">
            <AppCard v-for="(card, index) in cards" :key="index" :details="card" />
        </div>
        <div class="load">
            <button>LOAD MORE</button>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

main {
    min-height: 100px;
    border: 1px solid black;
    background-color: #1C1C1C;
    color: white;
    font-size: 50px;

    .title-container {
        width: 80%;
        margin: 0 auto;
        margin-bottom: 20px;

        .title {
            padding: 10px;
            margin-top: -20px;
            background-color: blue;
            color: white;
            font-size: 20px;
            width: fit-content;
        }
    }

    .container {
        width: 80%;
        margin: 0 auto;
        min-height: 100px;
        display: flex;
        flex-wrap: wrap;
        margin-bottom: 20px;
    }

    .load {
        width: 80%;
        margin: 0 auto;
        text-align: center;
        margin-bottom: 40px;

        button {
            background-color: blue;
            color: white;
            padding: 10px 50px;
        }
    }
}
</style>
