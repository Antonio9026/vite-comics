<script >
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBanner from './components/Appbanner.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppBanner,
    AppFooter
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppBanner></AppBanner>
  <AppFooter></AppFooter>
</template>

<style scoped></style>
