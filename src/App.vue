<script >
import AppHeader from './components/AppHeader.vue'
import AppHero from './components/AppHero.vue';
import AppMain from './components/AppHero.vue';
import AppFooter from './components/AppHero.vue';
export default {
  components: {
    AppHeader,
    AppHero,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppHero></AppHero>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style scoped></style>
