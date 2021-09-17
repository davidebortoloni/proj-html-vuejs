<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
    <!-- Bottone per tornare in cima alla pagina -->
    <a id="go-up" class="d-flex" href="#hero">
      <fa :icon="['fas', 'arrow-up']" />
    </a>
  </div>
</template>

<script>
// Importazione componenti
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  // Registrazione componenti
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "./assets/scss/style.scss";

// Stilizzazione bottone per tornare in cima alla pagina
#go-up {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  position: fixed;
  right: 50px;
  bottom: 85px;
  background-color: white;
  z-index: 3;
  justify-content: center;
  align-items: center;
  border: 1px solid rgb(100, 100, 100);
  color: rgb(100, 100, 100);
  text-decoration: none;
}
</style>
