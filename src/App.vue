<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
import * as db from './database/db.js'
export default {
  name: 'app',
  mounted: async function () {
    db.demoDocuments()
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
body {
  margin: 0px;
}
html {
    position: relative;
    min-height: 100%;
}
</style>
