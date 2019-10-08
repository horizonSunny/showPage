<template>
  <div id="app">
    <mainInfo />
  </div>
</template>

<script>
import mainInfo from './components/main.vue'

export default {
  name: 'app',
  components: {
    mainInfo
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
