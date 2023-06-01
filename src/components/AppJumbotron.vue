<script >

export default {
    name: "AppJumbotron",
}

</script>

<template>
    <div class="jumbo"></div>
</template>

<style lang="scss">
@use "../styles/partials/variables.scss" as *;

.jumbo {
    height: 300px;
    background-image: url(../../public/img/jumbotron.jpg);
    background-size: cover;
}
</style>