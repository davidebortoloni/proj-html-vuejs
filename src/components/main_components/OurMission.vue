<template>
  <div id="our-mission">
    <div class="container-fluid">
      <div class="row align-items-center">
        <div class="col-7"></div>

        <div class="col-5">
          <h2>
            learn more about our
            <span class="text-main">missions</span>
          </h2>
          <Divider />
          <p>
            Far far away, behind the word mountains, far from the countries
            Vokalia and Consonantia, there live the blind texts. Separated they
            live in Bookmarksgrove right at the coast of the Semantics, a large
            language ocean. Separated they live in Bookmarksgrove.
          </p>
          <button class="button btn-standard my-3">READ MORE</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Divider from "../_generals/Divider.vue";

export default {
  name: "OurMission",
  components: {
    Divider,
  },
};
</script>

<style scoped lang="scss">
</style>