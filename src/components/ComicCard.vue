<template>
  <div class="card-box">
      <img :src="comics.src" :alt="comics.series">
      <h6>{{comics.series}}</h6>
      
  </div>
</template>

<script>
export default {
    name: "ComicCard",
    props: ["comics"]
}
</script>

<style lang="scss" scoped>
    .card-box {
        width: calc(100% / 6);
        display: flex;
        padding: 5px 15px;
        background-color: darkmagenta;
        color: white;
    }


</style>