<script>

export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHRACTERS",
                    url: "#",
                    current: false
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    text: "MOVIE",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false
                },
                {
                    text: "NEW",
                    url: "#",
                    current: false
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false
                },
            ]
        }
    }
}

</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../../public/img/dc-logo.png" alt="">
            </div>

            <nav>
                <ul>
                    <li v-for="link in links">
                        <a href="" :class="link.current === true ? 'active' : ''">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

header {
    height: 80px;
    margin: 10px;

    .container {
        width: 80%;
        margin: 0 auto;
        display: flex;
        height: inherit;

        .logo {
            width: 30%;

            img {
                height: 100%;
            }
        }

        nav {
            width: 70%;
            display: flex;
            align-items: center;

            ul {
                list-style-type: none;
                width: 100%;
                display: flex;
                justify-content: space-between;

                a {
                    text-decoration: none;
                    color: black;

                    &.active,
                    &:hover {
                        color: $primary-color;
                        background-color: rgb(186, 186, 234);
                        border-bottom: 5px solid #0004ff;
                        padding: 10px;
                    }
                }
            }
        }
    }
}
</style>
