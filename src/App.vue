<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HomeView data="Leo is here!"  msg="we are iCan Lanka" />
  </div>
</template>

<script>
import HomeView from './components/HomeView.vue'

export default {
  name: 'App',
  components: { 
    HomeView
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
