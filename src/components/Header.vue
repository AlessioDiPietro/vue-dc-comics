<template>
  <header>
      <div class="box-header">

          <img src="@/assets/img/dc-logo.png" alt="DCLogo">

          <nav>
              <ul>
                  <li><a href="#"></a></li>
              </ul>
          </nav>


      </div>

  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return [
          {
              select: "CHARACTERS",
              firstOpt: "Batman",
              secondOpt:"joker"
          },
          {
              select: "COMICS",
              firstOpt: "Uscita 1",
              secondOpt:"Uscita 2"
          },
          {
              select: "MOVIES",
              firstOpt: "Arkam Asilium",
              secondOpt:"Suicide Squad"
          },
          {
              select: "TV",
              firstOpt: "Batman TheSeries",
              secondOpt:"joker L'INCORREGIBILE"
          },
          {
              select: "COLLECTIBLES",
              firstOpt: "ACTION-FIGURES Batman",
              secondOpt:"ACTION-FIGURES joker"
          },
          {
              select: "VIDEOS",
              firstOpt: "BACKSTAGE",
              secondOpt:"Meet THE DC STUDIOS"
          },
          {
              select: "FANS",
              firstOpt: "OUR SOCIAL",
              secondOpt:"FanBase"
          },
          {
              select: "NEWS",
              firstOpt: "LAST NEWS",
              secondOpt:"Weekly Highlights"
          },
          {
              select: "SHOP",
              firstOpt: "Merch",
              secondOpt:"Offerts"
          }
      ]
  }

}
// importazione file scss
import '../components/style/Commons.scss'
import '../components/style/BlueDC.scss'
</script>

<style lang="scss" scoped>
    .box-header {
        height: 115px;
        background-color: red;
        padding: 2% 17%;
        
    }
    
</style>