<script >
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBanner from './components/Appbanner.vue';
import AppFooter from './components/AppFooter.vue';
import AppHero from './components/AppHero.vue';

export default {
  components: {
    AppHeader,
    AppHero,
    AppMain,
    AppBanner,
    AppFooter
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppHero></AppHero>
  <AppMain></AppMain>
  <AppBanner></AppBanner>
  <AppFooter></AppFooter>
</template>

<style scoped></style>
