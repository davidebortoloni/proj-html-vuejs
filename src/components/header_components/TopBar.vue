<template>
  <div>
    <div class="container">
      <div class="row justify-content-between py-2 text-white">
        <div class="col-auto">(001)88451234 88455438</div>
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
  </div>
</template>

<script>
export default {
  name: "TopBar",
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";
a {
  color: white;
  &:hover {
    color: $mainColor;
  }
}
</style>
