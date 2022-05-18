<template>
  <div id="app">
    <AppHeader />
    <div class="banner"></div>
    <AppCurrentSeries />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppCurrentSeries from "./components/AppCurrentSeries.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppCurrentSeries,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";

main {
  height: 300px;
  background-color: black;
}

div.banner {
  background-image: url(./assets/img/jumbotron.jpg);
  background-size: 100%;
  height: 300px;
}
</style>
