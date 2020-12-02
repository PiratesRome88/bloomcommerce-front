<template>
  <div id="app">
      <b-navbar type="light" variant="light">
    <b-navbar-nav >
      <b-nav-item to="/">Home</b-nav-item> |
      <b-nav-item to="/about">About</b-nav-item>
      <b-nav-item to="/list">Catalogue</b-nav-item>
    </b-navbar-nav>
  </b-navbar>
    <router-view />
  </div>
</template>

<script>
import { BNavbar, BNavbarNav, BNavItem } from 'bootstrap-vue'

export default {
  name: "Root",
  components: {
    BNavbar,
    BNavbarNav,
    BNavItem
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
