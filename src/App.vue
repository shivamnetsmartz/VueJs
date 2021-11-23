<template>
<div id="app">
  <img alt="Vue logo" src="./assets/logo.png">
<!-- <Home data="Shivam Bhatia" msg="we are working on vuejs" />
  <Condition /> -->
  <ForLoop />
</div>
</template>

<script>

// import Home from './components/Home.vue'
// import Condition from './components/Condition.vue'
import ForLoop from './components/ForLoop.vue'

export default {
  name: 'App',
  components: {
    // Home,
    // Condition,
    ForLoop
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
