<template>
  <div id="app">
    <AppHeader />
    <main>questo è il main</main>
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
  height: 300px;
  background-color: black;
}
</style>
