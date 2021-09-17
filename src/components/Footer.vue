<template>
  <footer>
    <MainBar />
    <BottomBar />
  </footer>
</template>

<script>
import MainBar from "./footer_components/MainBar.vue";
import BottomBar from "./footer_components/BottomBar.vue";

export default {
  name: "Footer",
  components: {
    MainBar,
    BottomBar,
  },
};
</script>
