<template>
  <!-- Intestazione della pagina -->
  <div id="hero">
    <div class="container h-100">
      <div class="h-100 row align-items-center">
        <div class="col-6">
          <div class="content">
            <h4>17 YEARS OF EXPERIENCE</h4>
            <h2>
              We Are a
              <br />
              Web Design <span class="text-main">Agency</span>
            </h2>
            <Divider />
            <p>
              Far far away, behind the word mountains, far from the countries
              Vokalia and Consonantia, there live the blind texts. Separated
              they live in Bookmarksgrove right at the coast of the Semantics, a
              large language ocean. Separated they live in Bookmarksgrove.
            </p>
            <button class="button btn-reverse my-4">READ MORE</button>
            <ul class="my-5 p-0">
              <li><a href="#">FACEBOOK</a></li>
              <li>-</li>
              <li><a href="#">INSTAGRAM</a></li>
              <li>-</li>
              <li><a href="#">YOUTUBE</a></li>
              <li>-</li>
              <li><a href="#">TWITTER</a></li>
            </ul>
          </div>
        </div>
        <div class="col-6">
          <img src="../../assets/img/Group-36-2x.png" alt="Girl staff" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Divider from "../_generals/Divider.vue";

export default {
  name: "Hero",
  components: {
    Divider,
  },
};
</script>

<style scoped lang="scss">
// Importazione variabili
@import "../../assets/scss/_vars.scss";

// Stilizzazione hero
#hero {
  height: 1100px;
  overflow: hidden;
  .content {
    position: relative;
    top: 50px;
    h2 {
      font-weight: 700 !important;
    }
    ul {
      font-family: "Quicksand", sans-serif;
      font-weight: 700;
      font-size: 14px;
      list-style-type: none;
      li {
        display: inline-block;
        color: $thirdColor;
        padding-right: 10px;
        a {
          color: $thirdColor;
          text-decoration: none;
          &:hover {
            color: $mainColor;
          }
        }
      }
    }
  }
  img {
    width: 190%;
    position: relative;
    top: 70px;
    right: 170px;
  }
}
</style>