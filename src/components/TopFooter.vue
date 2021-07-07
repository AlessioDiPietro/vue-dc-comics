<template>
  <div class="topfooter-box">

      <ul>
          <li v-for="(items, index) in card" :key="index">
              <img :src="getSrc(items.img)" :alt="items.text">
              <h6>{{items.text}}</h6>

          </li>
      </ul>

  </div>
</template>

<script>
export default {
    name: 'TopFooter',
    data(){
        return{
            card: [
                {
                    text: 'DIGITAL COMICS',
                    img: 'buy-comics-digital-comics.png'

                },
                {
                    text: 'DC MERCHANDISE',
                    img: 'buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    img: 'buy-dc-power-visa.svg'
                },
                
            ]
        }
    },
    methods: {
        getSrc(img){
            return require('../assets/img/' + img)
        }
    }

}
</script>

<style lang="scss">
@import '../components/style/BlueDC.scss';
.topfooter-box {
    height: 150px;
    color: white;
    background-color:$bluedc;
    z-index: 1;
    position: relative;
    padding: 3%;

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;

        li {
            margin: 0 1%;
            list-style: none;
            display: flex;
            align-items: center;
            
            img {
                width: 60px;;
                margin-right: 3%;
            }
        }
    }

}

</style>