<template>
  <div class="bottfooter-box">
      <button>SIGN-UP NOW!</button>
      <div class="social-box">
          <span>FOLLOW US</span>
          <img src="@/assets/img/footer-facebook.png" alt="#">
          <img src="@/assets/img/footer-twitter.png" alt="#">
          <img src="@/assets/img/footer-youtube.png" alt="#">
          <img src="@/assets/img/footer-pinterest.png" alt="#">
          <img src="@/assets/img/footer-periscope.png" alt="#">
      </div>
  </div>
</template>

<script>
export default {
    name: "BottFooter",
}
</script>

<style lang="scss" scoped>
    @import '../components/style/BlueDC.scss';

    .bottfooter-box {
        background-color: #303030;
        color: $bluedc;
        position: relative;
        z-index: 1;
        height: 110px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 2% 17%;

        button{
            color: white;
            font-size: 20px;
            border: 3px solid $bluedc;
            background-color: transparent;
            padding: 10px 15px;
        }

        .social-box{
             span {
                 vertical-align: 10px;
                 margin: 0 15px;
                 font-weight: 900;
             }
             img {
                 margin: 0 15px;
             }
        }


    }

</style>