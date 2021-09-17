<template>
  <footer>
    <!-- Contenuto principale del footer -->
    <MainBar />
    <!-- Barra inferiore della pagina -->
    <BottomBar />
  </footer>
</template>

<script>
// Importazione componenti
import MainBar from "./footer_components/MainBar.vue";
import BottomBar from "./footer_components/BottomBar.vue";

export default {
  name: "Footer",
  // Registrazione componenti
  components: {
    MainBar,
    BottomBar,
  },
};
</script>
