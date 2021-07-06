<template>
  <div class="midfooter-box">

    <aside class="left">
        <ul>
            <li class="title">DC COMICS</li>
            <li v-for="(items, index) in comics" :key="index">{{items}}</li>
        </ul>

        <ul>
            <li class="title">DC</li>
            <li v-for="(items, index) in dc" :key="index">{{items}}</li>
        </ul>

        <ul>
            <li class="title">SITES</li>
            <li v-for="(items, index) in sites" :key="index">{{items}}</li>
        </ul>

        <ul>
            <li class="title">SHOP</li>
            <li v-for="(items, index) in shop" :key="index">{{items}}</li>
        </ul>
    </aside>


    <aside class="right">
        <img src="../assets/img/dc-logo-bg.png" alt="">
    </aside>



  </div>
</template>

<script>
export default {
    name: "MidFooter",
    data(){
        return{
            comics: 
                {
                    text1: "Characters", 
                    text2: "Comics", 
                    text3: "Movies", 
                    text4: "TV", 
                    text5: "Games", 
                    text6: "Videos", 
                    text7: "News" 
                }
            ,
            dc: 
                {
                    text1: "T O U", 
                    text2: "Privacy policy (New)", 
                    text3: "AD Choices", 
                    text4: "Advertising", 
                    text5: "Jobs", 
                    text6: "Subscriptions", 
                    text7: "Talent Workshops",
                    text8: "CPSC Certificates",
                    text9: "Ratings",
                    text10: "Shop Help",
                    text11: "Contact Us"
                },
            sites: 
                {
                    text1: "DC", 
                    text2: "MAD Magazine", 
                    text3: "DC Kids", 
                    text4: "DC Universe", 
                    text5: "DC Power Visa" 
                },
            shop: 
                {
                    text1: "Shop DC", 
                    text2: "Shop DC Collectibles"
                    
                }
        }
    }

}
</script>

<style lang="scss" scoped>
.midfooter-box {
    background-image: url('../assets/img/footer-bg.jpg');
    height: 370px;
    padding: 2% 16%;
    background-size: cover;
    display: flex;
    justify-content: space-between;
    position: relative;

    .left{
        width: 30% ;
        display: flex;

        
        ul{
            margin: 0 20px;

            .title {
                color: white;
                margin-bottom: 15px;
                font-size: 20px;
            }
            li{
                list-style: none;
                color: grey;

                
            }
        }

    }


    .right{
        position: absolute;
        right: 15%;
        top: -94px;;
    }




    
}

</style>