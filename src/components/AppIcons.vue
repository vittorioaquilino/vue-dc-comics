<template>
  <div class="icon-container">
      <div class="container">
        <div class="icon-list">
            <img :src="iconsObj.thumb" alt="">
        </div>
        <h5>{{ iconsObj.series}}</h5>
      </div>
  </div>
</template>

<script>
export default {
    name: "AppIcons",
    props: ["iconsObj"],
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.icon-container {
  width: calc(100% / 6 - 20px);
  margin: 0 10px;

  .icon-list {
    margin-top: 2rem;
    margin-bottom: .5rem;
      
      img {
        width: 150px;
        height: 150px;
      }

    }
  h5 {
    text-transform: uppercase;
    color: white;
    font-size: .6rem;
    font-weight: 300;
  }
}

</style>