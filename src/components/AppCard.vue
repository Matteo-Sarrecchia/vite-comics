<script >

export default {
    name: "AppCard",
    props: {
        details: Object
    }
}

</script>

<template>
    <div class="card">
        <div class="img-row">
            <img :src="details.thumb" alt="">
        </div>
        <div class="text">{{ details.series }}</div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

.card {
    min-height: 100px;
    width: 180px;
    margin: 10px auto;
    border: 1px solid rgb(255, 255, 255);

    .img-row {
        width: 180px;
        height: 180px;

        img {
            height: 180px;
            width: 180px;
            display: block;
        }

    }

    .text {
        margin: 10px;
        text-align: center;
        font-size: 15px;
    }
}
</style>
