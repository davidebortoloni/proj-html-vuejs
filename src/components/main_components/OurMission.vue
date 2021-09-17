<template>
  <div id="our-mission">
    <div class="container-fluid">
      <div class="row align-items-center">
        <div class="col-7">
          <div class="images w-100">
            <div class="back">
              <img
                class="w-100"
                src="@/assets/img/busy-architect-PYVKWM4-1024x872.jpg"
                alt="Architect"
              />
              <div class="overlay"></div>
            </div>
            <div class="front">
              <img
                class="w-100"
                src="@/assets/img/businesswoman-analysing-document-P8WSNMC-1024x820.jpg"
                alt="Business Woman"
              />
            </div>
          </div>
        </div>
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
@import "../../assets/scss/_vars.scss";

.images {
  position: relative;
  top: 40px;
  right: 40px;
  display: flex;
  justify-content: center;
  .front,
  .back {
    border-radius: 20px;
    overflow: hidden;
    width: 80%;
    box-shadow: 3px 3px 15px 0 $sixthColor;
  }
  .back {
    position: absolute;
    top: -80px;
    left: 0;
    .overlay {
      position: absolute;
      z-index: 1;
      opacity: 0.8;
      top: 0px;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, $secondaryColor, $mainColor);
    }
  }
  .front {
    position: relative;
    z-index: 1;
  }
}
</style>