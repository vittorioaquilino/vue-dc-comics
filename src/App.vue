<template>
  <div id="app">
    <!-- header -->
    <AppHeader />
    <!-- main -->
  <main>
    <div class="container main__top">
      --> Content goes here -->
    </div>
  </main>
    <AppPreFooter />
    <!-- footer -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppPreFooter from "./components/AppPreFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppPreFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";

main {
  height: 100px;
  background-color: black ;
  color: white;
  display: flex;
  align-items: center;
}


</style>
