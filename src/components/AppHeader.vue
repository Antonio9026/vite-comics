<script >

export default {
  name: "AppHeader",
  Data() {
    return {
      links: [
        {
          text: "CHARACTERS"
        }, {
          text: "COMICS"
        }, {
          text: "MOVIES"
        }, {
          text: "TV"
        }, {
          text: "GAMES"
        }, {
          text: "COLLECTIBLES"
        }, {
          text: "VIDEOS"
        }, {
          text: "FANS"
        }, {
          text: "NEWS"
        }, {
          text: "SHOP"
        },
      ]
    }
  },
  
}

</script>

<template>
  <div class="header-container">
    <div class="header-logo">
      <a href="#"><img src="../assets/img/dc-logo.png" alt=""></a>
    </div>
    <nav>
      <ul>
        <li v-for="link in links"><a href="">{{ link.text }}</a></li>
      </ul>
    </nav>

  </div>
</template>

<style scoped></style>
