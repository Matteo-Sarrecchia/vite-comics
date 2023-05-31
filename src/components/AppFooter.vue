<script >

export default {
    name: "AppFooter",
}

</script>

<template>
    <footer>

        <!-- container -->
        <div class="container">

            <!-- contatti -->
            <div class="contatti">
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
                            <h3>DC</h3>
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
                            <h3>SITES</h3>
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

            <!-- logo -->
            <div class="logo"></div>
        </div>


        <!-- FOLLOW -->
        <div class="follow">
            <div class="container-follow">
                <div class="col-button">
                    <button>SIGN-IP NOW!</button>
                </div>

                <div class="col-link">
                    <ul>
                        <li>
                            <h3>FOLLOW US</h3>
                        </li>
                        <li>
                            <a href="">
                                <img src="../../public/img/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../../public/img/footer-periscope.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../../public/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../../public/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../../public/img/footer-youtube.png" alt="">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>



<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

footer {
    min-height: 100px;
    background-image: url(../../public/img/footer-bg.jpg);
    background-size: cover;
    border: 1px solid black;

    .container {
        width: 80%;
        height: 300px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;

        .logo {
            width: 35%;
            height: 100%;
            background-image: url(../../public/img/dc-logo-bg.png);
            background-size: cover;
            background-position: center;
        }

        .contatti {
            padding: 20px 0;
            min-height: 100px;
            width: 50%;
            display: flex;

            .col {
                width: 30%;
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

    }

    // FOLLOW SECTION
    .follow {
        height: 100px;
        background-color: black;
        display: flex;
        justify-content: space-between;

        .container-follow {
            width: 80%;
            margin: 0 auto;
            display: flex;
        }

        .col-button {
            width: 70%;
            display: flex;
            align-items: center;

            button {
                padding: 10px;
                background: none;
                color: white;
                border: 1px solid blue;

                &:hover {
                    background-color: rgb(186, 186, 234);
                    color: $primary-color;
                }
            }
        }

        .col-link {
            width: 30%;
            display: flex;
            align-items: center;

            h3 {
                color: $primary-color;
            }

            ul {
                list-style-type: none;
                width: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                li {
                    padding: 5px;
                }
            }
        }
    }
}
</style>
