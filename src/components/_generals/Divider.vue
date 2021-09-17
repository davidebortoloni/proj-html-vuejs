<template>
  <!-- Divisore tra elementi -->
  <div class="divider my-4">&nbsp;</div>
</template>

<script>
export default {
  name: "Divider",
};
</script>

<style scoped lang="scss">
// Importazione variabili
@import "../../assets/scss/_vars.scss";

// Stilizzazione divisore
.divider {
  position: relative;
  &::before,
  &::after {
    content: "";
    position: absolute;
    border-radius: 20px;
    height: 5px;
    top: 0;
    background-image: linear-gradient(to right, $secondaryColor, $mainColor);
  }
  &::before {
    width: 10px;
    left: 0;
  }
  &::after {
    width: 50px;
    left: 15px;
  }
}
</style>