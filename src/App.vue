<template>
  <div id="app">
    
    <header>
        <myHeaderDC/>
    </header>

    <!-- MAIN -->

    <!-- FOOTER -->
</template>

<script>
import myHeaderDC from './components/myHeaderDC.vue'

export default {
  name: 'App',
  components: {
    myHeaderDC,
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
  margin-top: 60px;
}
</style>
