<template>
  <div class="prefooter">
    <div class="container">
      <ul class="icons-list">
        <li
        v-for="(element, index) in icons"
        :key="index"
        >
          <img :src="require(`../assets/img/${element.img}`)" alt="">
          <h3>{{ element.text }}</h3>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppPreFooter",
  data: function () {
    return {
      icons: [
        {
          img: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "DC Merchandise",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "subscription",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "Comic shop locator",
        },
        {
          img: 'buy-dc-power-visa.svg',
          text: "DC power visa",
        }
      ],
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.prefooter {
  background-color: $brand-primary-color;

  .icons-list {
    display: flex;

    li {
      width: calc(100% / 5);
      display: flex;
      align-items: center;
      padding: 2rem;
    }

    img {
      width: 30px;
      margin-right: .4rem;
    }

    h3 {
      font-size: .8rem;
      font-weight: 300;
      text-transform: uppercase;
      color: white;
    }
  }
}
</style>