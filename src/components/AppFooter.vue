<script >

export default {
    name: "AppFooter",
}

</script>

<template>
    <footer>
        <!-- logo -->
        <div class="container">
            <div class="logo">
                <!-- <img src="../../public/img/dc-logo-bg.png" alt=""> -->
            </div>

            <div class="menu">
                <div class="col">
                    <ul>
                        <li>
                            <h3>DC COMICS</h3>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>

                    <ul>
                        <li>
                            <h3>SHOP</h3>
                        </li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>

                    </ul>
                </div>

                <div class="col">
                    <ul>
                        <li>
                            <h3>DC COMICS</h3>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </div>
                <div class="col">
                    <ul>
                        <li>
                            <h3>DC COMICS</h3>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </div>
            </div>

            <div class="follow">

            </div>

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

footer {
    min-height: 500px;
    background-image: url(../../public/img/footer-bg.jpg);
    background-size: cover;
    border: 1px solid black;

    .container {
        width: 80%;
        height: 500px;
        margin: 0 auto;
        border: 1px solid white;
        position: relative;

        .logo {
            width: 45%;
            height: 100%;
            position: absolute;
            text-align: end;
            top: 0;
            right: 0;
            background-image: url(../../public/img/dc-logo-bg.png);
            background-size: cover;
            border: 1px solid white;

            img {
                width: 100%;
            }
        }

        .menu {
            min-height: 100px;
            width: 50%;
            border: 1px solid white;
            display: flex;

            .col {
                width: calc(100% / 3);
                color: grey;

                ul {
                    list-style-type: none;
                    margin-bottom: 10px;

                    h3 {
                        margin-bottom: 10px;
                        color: white;
                    }
                }
            }
        }

        .follow {
            height: 100px;
            background-color: black;
        }
    }
}
</style>
