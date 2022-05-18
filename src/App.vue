<template>
    <div id="app">
      <!-- header -->
      <AppHeader />
      <!-- main -->
      <AppMain />
      <!-- prefooter -->
      <AppPreFooter />
      <!-- footer -->
      <AppFooter />
    </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppPreFooter from "./components/AppPreFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppPreFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";



</style>
