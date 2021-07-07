<template>
  <div class="container">
      
      <ComicCard
       v-for="(items,index) in comicItems" 
       :key="index" 
       :comics="items"/>

      <button>LOAD MORE</button>

  </div>
</template>

<script>
import ComicCard from "@/components/ComicCard.vue"
import ComicsInfo from "@/components/data/ComicsInfo.js"
export default {
    name: 'MainContent',
    components: {
        ComicCard,
    },
    data(){
        return {
            comicItems: ComicsInfo
            
        }
    }


}
</script>

<style lang="scss" scoped>
@import '../components/style/BlueDC.scss';
    .container {
        padding: 55px 16%;
        background-color: black;
        color: white;
        padding: 3% 24%; 
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        
        button{
            background-color: $bluedc;
            border: none;
            padding: 5px 30px;
            font-size: 18px;
            margin-top: 25px;
            cursor: pointer;
            color: white;
        }
    }


</style>