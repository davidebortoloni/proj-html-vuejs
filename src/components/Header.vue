<template>
  <div>
    <TopBar id="headerTopBar" />
    <Nav id="headerNav" />
  </div>
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
#headerTopBar {
  background-color: #3d3d3d;
}
</style>
