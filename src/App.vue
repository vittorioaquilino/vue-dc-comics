<template>
  <div id="app">
    <!-- header -->
    <AppHeader />
    <!-- main -->
  <main>
    questo è il main
    </main>
    <div class="jumbotron">jumbo</div>
    <!-- footer -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";

main {
  height: 100px;
  background-color: black ;
  color: white;
}

.jumbotron {
  height: 100px;
  background-color: #0082f9;
}
</style>
