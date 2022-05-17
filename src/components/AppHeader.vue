<template>
  <header class="header">
    <div class="header__logo">
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <div class="navigation__bar"></div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.header {
  width: $general-width-page;
  margin: $general-center-page;
  background-color: red;
  &__logo {
    img {
      width: 8%;
    }
  }
}
</style>
