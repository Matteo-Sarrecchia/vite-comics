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
    width: calc(100% / 6 - 20px);
    margin: 10px auto;

    .img-row {
        max-width: 180px;
        max-height: 180px;

        img{
            width: 180px;
            max-height: 180px;
        }
    }

    .text {
        margin: 10px;
        text-align: center;
        font-size: 15px;
    }
}
</style>
