<template>
  <div id="app">
    
    <header>
        <myHeaderDC/>
    </header>

    <main>
      <MainContent/>
      <ServiceBanner/>
    </main>

    <footer>
      <FooterLink/>
    </footer>

    </div>
</template>

<script>
import myHeaderDC from './components/myHeaderDC.vue'
import MainContent from './components/MainContent.vue'
import ServiceBanner from './components/ServiceBanner.vue'
import FooterLink from './components/FooterLink.vue'

export default {
  name: 'App',
  components: {
    myHeaderDC,
    MainContent,
    ServiceBanner,
    FooterLink,
  }
}
</script>

<style lang="scss">
@import './style/commons.scss';
</style>
