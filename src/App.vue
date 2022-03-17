<template>
  <div id="app">
    <ApiSites/>
  </div>
</template>

<script>
import ApiSites from './components/ApiSites'

export default {
  name: 'App',
  components: {
    ApiSites
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
