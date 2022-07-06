<template>
  <div id="app">
    
    <header>
        <myHeaderDC/>
    </header>

    <main>
      <MainContent/>
      <ServiceBanner/>
    </main>

    <!-- FOOTER -->
    </div>
</template>

<script>
import myHeaderDC from './components/myHeaderDC.vue'
import MainContent from './components/MainContent.vue'
import ServiceBanner from './components/ServiceBanner.vue'

export default {
  name: 'App',
  components: {
    myHeaderDC,
    MainContent,
    ServiceBanner,
  }
}
</script>

<style lang="scss">
@import './style/commons.scss'
</style>
