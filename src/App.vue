<template>
  <div id="app">
    <!-- barra ricerca -->
    <Header/>

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
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import TopFooter from './components/TopFooter.vue'
import MidFooter from './components/MidFooter.vue'
import BottFooter from './components/BottFooter.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    TopFooter,
    MidFooter,
    BottFooter
  }
}
</script>

<style lang="scss">
</style>
