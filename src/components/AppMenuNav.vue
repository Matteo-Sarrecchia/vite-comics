<script >

export default {
    name: "AppMenuNav"
}

</script>

<template>
    <section class="appMenuNav">

        <div class="container">
            <div class="col">
                <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                <a href="">DIGITAL COMICS</a>
            </div>

            <div class="col">
                <img src="../../public/img/buy-comics-merchandise.png" alt="">
                <a href="">DC MERCHANDISE</a>
            </div>

            <div class="col">
                <img src="../../public/img/buy-comics-subscriptions.png" alt="">
                <a href="">SUBSCRIPTION</a>
            </div>

            <div class="col">
                <img src="../../public/img/buy-comics-shop-locator.png" alt="">
                <a href="">COMIC SHOP LOCATOR</a>
            </div>

            <div class="col">
                <img src="../../public/img/buy-dc-power-visa.svg" alt="">
                <a href="">DC POWER VISA</a>
            </div>

        </div>

    </section>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

.appMenuNav {
    background-color: #0282F9;
    min-height: 100px;

    .container {
        width: 80%;
        margin: 0 auto;
        display: flex;
        align-items: center;

        .col {
            width: calc(100% / 5);
            height: 100px;
            display: flex;
            align-items: center;
            justify-content: center;

            img {
                width: 40px;
                margin: 10px;
            }

            a {
                text-decoration: none;
                color: white;
            }
        }
    }
}
</style>
