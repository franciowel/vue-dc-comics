<template>
  <div id="app">
    
    <header>
        <myHeaderDC/>
        <SponsorBanner/>
    </header>

    <main>
      <MainContent/>
      <ServiceBanner/>
    </main>

    <footer>
      <FooterLink/>
      <FooterBottom/>
    </footer>

    </div>
</template>

<script>
import myHeaderDC from './components/myHeaderDC.vue'
import MainContent from './components/MainContent.vue'
import ServiceBanner from './components/ServiceBanner.vue'
import FooterLink from './components/FooterLink.vue'
import FooterBottom from './components/FooterBottom.vue'
import SponsorBanner from './components/SponsorBanner.vue'

export default {
  name: 'App',
  components: {
    myHeaderDC,
    SponsorBanner,
    MainContent,
    ServiceBanner,
    FooterLink,
    FooterBottom,
  }
}
</script>

<style lang="scss">
@import './style/commons.scss';
</style>
