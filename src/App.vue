<template>
  <div id="app">
    <Header/>
    <Home/>
    <About/>
    <Works/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Home from "./components/Home.vue";
import About from "./components/About.vue";
import Works from "./components/Works.vue";

export default {
  name: 'App',
  components: {
    Header,
    Home,
    About,
    Works,
  }
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>
