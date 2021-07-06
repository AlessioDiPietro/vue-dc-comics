<template>
  <header>
      <div class="box-header">

          <img src="@/assets/img/dc-logo.png" alt="DCLogo">

          <nav>
              <ul>
                  <li v-for="(item, index) in navig" :key="index">
                      <a href="#">{{item.select}}</a>
                    </li>
              </ul>
          </nav>


      </div>

  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
        navig: [
          {
              select: "CHARACTERS",
              firstOpt: "Batman",
              secondOpt:"joker",
              status: false
          },
          {
              select: "COMICS",
              firstOpt: "Uscita 1",
              secondOpt:"Uscita 2",
              status: false
          },
          {
              select: "MOVIES",
              firstOpt: "Arkam Asilium",
              secondOpt:"Suicide Squad",
              status: false
          },
          {
              select: "TV",
              firstOpt: "Batman TheSeries",
              secondOpt:"joker L'INCORREGIBILE",
              status: false
          },
          {
              select: "COLLECTIBLES",
              firstOpt: "ACTION-FIGURES Batman",
              secondOpt:"ACTION-FIGURES joker",
              status: false
          },
          {
              select: "VIDEOS",
              firstOpt: "BACKSTAGE",
              secondOpt:"Meet THE DC STUDIOS",
              status: false
          },
          {
              select: "FANS",
              firstOpt: "OUR SOCIAL",
              secondOpt:"FanBase",
              status: false
          },
          {
              select: "NEWS",
              firstOpt: "LAST NEWS",
              secondOpt:"Weekly Highlights",
              status: false
          },
          {
              select: "SHOP",
              firstOpt: "Merch",
              secondOpt:"Offerts",
              status: false
          }
        ]
      }
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
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {    
        height: 100%;
        }

        li {
            display: inline-block;
            margin: 0 15px;
            cursor: pointer;
            padding: 47px 0;

            &:hover {
                border-bottom: 3px solid black;
                padding: 44px 0;

            }

            a {
                color: rgb(68, 67, 67);
                text-decoration: none;
            }
        }
    }
    
</style>