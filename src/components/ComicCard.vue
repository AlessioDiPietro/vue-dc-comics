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
        padding: 5px 15px;
        color: white;
        img {
            width: 100%;
            margin-bottom: 5px;
        }
        h6{
            font-size: 12px;
            margin-bottom: 15px;
        }
    }

</style>