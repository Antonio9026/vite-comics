<script >
import cardsList from "./db/comics"
import AppHeader from './components/AppHeader.vue';
import AppcardList from './components/AppcardList.vue';
import AppBanner from './components/AppBanner.vue';
import AppFooter from './components/AppFooter.vue';
import AppHero from './components/AppHero.vue';

export default {
  components: {
    AppHeader,
    AppHero,
    AppcardList,
    AppBanner,
    AppFooter
  },
  data() {
    return {
      cardsList,

    };
  },
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppHero></AppHero>
  <main>
    <button class="current-btn"><strong>CURRENT SERIES</strong></button>
    <div class="card-wrapper">
      <AppcardList :thumb="card.thumb" :series="card.series" v-for="card in cardsList"></AppcardList>
      <button class="load-button"><strong>LOAD MORE</strong></button>
    </div>

  </main>

  <AppBanner></AppBanner>
  <AppFooter></AppFooter>
</template>

<style lang="scss" scoped>
main {
  background-color: #1c1c1c;
  position: relative;

  .current-btn {
    width: 210px;
    height: 30px;
    position: absolute;
    top: -15px;
    left: 190px;
    border-radius: 0;
    background-color: #0282f9;
    border: 0;
    color: white;
    font-size: large;
  }

  .card-wrapper {
    display: flex;
    flex-wrap: wrap;
    width: 70%;
    margin: 0 auto;
    padding-top: 20px;
    justify-content: center;

    .load-button {
      width: 140px;
      height: 20px;
      margin: 20px 0;
      border-radius: 0;
      background-color: #0282f9;
      border: 0;
      color: white;
      font-size: small;
    }
  }
}





</style>
