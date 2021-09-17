<template>
  <div id="bottom-bar">
    <div class="row justify-content-between py-2">
      <div class="col-auto copy">© 2021 PHLOX BUSINESS THEME.</div>
      <div class="col-auto">
        <a href="#">
          <fa class="mx-3 clickable" :icon="['fab', 'facebook-f']" />
        </a>
        <a href="#">
          <fa class="mx-3 clickable" :icon="['fab', 'twitter']" />
        </a>
        <a href="#">
          <fa class="mx-3 clickable" :icon="['fab', 'pinterest-p']" />
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomBar",
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";

#bottom-bar {
  padding: 35px 30px;
  background: linear-gradient(90deg, $thirdColor, $fourthColor);
  @import "../../assets/scss/_vars.scss";
  a {
    color: $fifthColor;
    &:hover {
      color: $sixthColor;
    }
  }
  .copy {
    font-size: 14px;
    font-family: "Ubuntu", sans-serif;
    font-weight: 400;
    color: $fifthColor;
  }
}
</style>