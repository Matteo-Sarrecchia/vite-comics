<script >

export default {
    name: "AppMain",
}

</script>

<template>
    <main>
        ...parte centrale...
    </main>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

main {
    min-height: 100px;
    border: 1px solid black;
    text-align: center;
    background-color: black;
    color: white;
    font-size: 50px;
}
</style>
