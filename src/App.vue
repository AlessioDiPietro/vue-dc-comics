<template>
  <div id="app">
    <!-- barra ricerca -->
    <Header/>

    <!-- jumbotron -->
    <Jumbo/>

    <!-- corpo pagina -->
    <main>
      <MainContent/>
    </main>

    <!-- piè di pagina -->
    <footer>
      <TopFooter/>
      <MidFooter/>
      <BottFooter/>
    </footer>

  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import MainContent from '@/components/MainContent.vue'
import TopFooter from '@/components/TopFooter.vue'
import MidFooter from '@/components/MidFooter.vue'
import BottFooter from '@/components/BottFooter.vue'
import Jumbo from '@/components/Jumbo.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    TopFooter,
    MidFooter,
    BottFooter,
    Jumbo
  }
}
</script>

<style lang="scss">
    @import './components/style/Commons.scss';
</style>
