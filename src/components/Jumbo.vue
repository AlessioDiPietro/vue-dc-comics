<template>
  <section class="jumbo">

      <div class="note">CURRENT SERIES</div>

  </section>
</template>

<script>
export default {
    name: "Jumbo"

}
</script>

<style lang="scss" scoped>
@import "../components/style/BlueDC.scss";
    .jumbo {
        background-image: url("../assets/img/jumbotron.jpg");
        height: 400px;
        background-size: cover;
        position: relative;

        .note {
            padding: 10px 15px;
            color:white;
            font-size: larger;
            background-color: $bluedc;
            border-radius: 10px;
            position: absolute;
            bottom: 0px;
            left: 24%;
            transform:translate(0, 50%)
        }
    }

</style>