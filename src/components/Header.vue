<template>
  <header>
    <TopBar id="headerTopBar" />
    <Nav id="headerNav" />
  </header>
</template>

<script>
import TopBar from "./header_components/TopBar.vue";
import Nav from "./header_components/Nav.vue";

export default {
  name: "Header",
  components: {
    TopBar,
    Nav,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

header {
  position: fixed;
  z-index: 2;
  width: 100%;
  #headerTopBar {
    background-color: $thirdColor;
  }
  #headerNav {
    background-color: $fifthColor;
  }
}
</style>
