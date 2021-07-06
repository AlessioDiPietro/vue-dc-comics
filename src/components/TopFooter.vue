<template>
  <div class="topfooter-box">

      <ul>
          <li v-for="(items, index) in card" :key="index">
              <img :src="items.img" :alt="items.text">
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
                    img: '../assets/img/buy-comics-digital-comics.png'

                },
                {
                    text: 'DC MERCHANDISE',
                    img: '../assets/img/buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: '../assets/img/buy-comics-subscription.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: '../assets/img/buy-comics-digital-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    img: '../assets/img/buy-dc-power-visa.png'
                },
                
            ]
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

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;
        margin: 0px 13%;

        li {
            margin: 0 2%;
            list-style: none;
            display: inline-block;
            
            h4 {
                display: inline-block;
            }
        }
    }

}

</style>