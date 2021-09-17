<template>
  <header>
    <!-- Barra superiore della pagina -->
    <TopBar id="headerTopBar" />
    <!-- Menù principale della pagina -->
    <Nav id="headerNav" />
  </header>
</template>

<script>
// Importazione componenti
import TopBar from "./header_components/TopBar.vue";
import Nav from "./header_components/Nav.vue";

export default {
  name: "Header",
  // Registrazione componenti
  components: {
    TopBar,
    Nav,
  },
};
</script>

<style scoped lang="scss">
// Importazione variabili
@import "../assets/scss/_vars.scss";

// Stilizzazione header
header {
  position: fixed;
  z-index: 2;
  width: 100%;
  // Barra superiore
  #headerTopBar {
    background-color: $thirdColor;
  }
  // Menù principale
  #headerNav {
    background-color: $fifthColor;
  }
}
</style>
