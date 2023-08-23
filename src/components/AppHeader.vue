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
        <li v-for="link in links">
          <a href="#" :class="{active: link.text === 'COMICS'}">{{ link.text }}</a>
        </li>
      </ul>
    </nav>

  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.container {
  justify-content: space-between;

  .header-logo {
    height: 100px;
    padding: 15px 0;

    a {
      height: 75px;
    }

  }

  ul {
    display: flex;
    height: 100%;
    gap: 10px;
    margin-right: 30px;

    li {
      font-size: 10px;
      font-weight: 700;

      a {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100%;
        color:$color-nav-link;
      }
      .active{
        color:#0282f9;
        border-bottom: 5px solid;
        border-color:#0282f9;
        height: 100px;
      }

    }
  }
}
</style>
