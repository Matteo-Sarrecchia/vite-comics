<script >
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppMenuNav from './components/AppMenuNav.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppMenuNav,
    AppFooter
  }
}

</script>

<template>
  <AppHeader />
  <AppMain />
  <AppMenuNav />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
@use "./styles/partials/variables.scss" as *;
</style>