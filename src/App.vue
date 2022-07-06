<template>
  <div id="app">
    
    <header>
        <myHeaderDC/>
    </header>

    <main>
      <MainContent/>
      <!-- BLUEJUMBO -->
    </main>

    <!-- FOOTER -->
    </div>
</template>

<script>
import myHeaderDC from './components/myHeaderDC.vue'
import MainContent from './components/MainContent.vue'

export default {
  name: 'App',
  components: {
    myHeaderDC,
    MainContent,
  }
}
</script>

<style lang="scss">
@import './style/commons.scss'
</style>
