<template>
  <div id="app">
    <menu-nav />
    <div style="margin: 0 0 0 320px">
      <navi-bar />
      <router-view />
      <img alt="Vue logo" src="@/assets/logo.png" />
      <footer-nav />
    </div>
  </div>
</template>

<script>
import MenuNav from "@/components/layout/MenuNav.vue";
import NaviBar from "@/components/layout/HeaderNavBar.vue";
import FooterNav from "@/components/layout/FooterNavBar.vue";

export default {
  name: "App",
  components: {
    MenuNav,
    NaviBar,
    FooterNav,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
