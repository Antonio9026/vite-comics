<script >

export default {
  name: "AppHeader",
  data() {
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
  <div class="container">
    <div class="header-logo">
      <a href="#"><img src="../assets/img/dc-logo.png" alt=""></a>
    </div>
    <nav>
      <ul>
        <li 
        v-for="link in links">
          <a href="">{{ link.text }}</a>
        </li>
      </ul>
    </nav>

  </div>
</template>

<style scoped>
.container{
  justify-content: space-between;
}
.header-logo{
  height: 75px;
  padding: 15px 0;
}
a{
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  color: black;
}
ul{
  display: flex;
  height: 100%;
  gap: 20px;
}
a{
height: 75px;
}
li{
  font-size: 10px;
  font-weight: 700;
}
</style>
