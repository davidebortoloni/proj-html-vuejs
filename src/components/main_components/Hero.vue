<template>
  <div id="hero">
    <div class="back h-100">
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
              <div class="divider my-4">&nbsp;</div>
              <p>
                Far far away, behind the word mountains, far from the countries
                Vokalia and Consonantia, there live the blind texts. Separated
                they live in Bookmarksgrove right at the coast of the Semantics,
                a large language ocean. Separated they live in Bookmarksgrove.
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
            <img src="../../assets/img/Group-36-2x.png" alt="aaa" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";

#hero {
  height: 1150px;
  overflow: hidden;
  .content {
    position: relative;
    top: 50px;
    .divider {
      position: relative;
      &::before,
      &::after {
        content: "";
        position: absolute;
        border-radius: 20px;
        height: 5px;
        top: 0;
        background-image: linear-gradient(
          to right,
          $secondaryColor,
          $mainColor
        );
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
    p {
      font-family: "Ubuntu", sans-serif;
      font-weight: 300;
      font-size: 16px;
      color: $thirdColor;
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
    top: 100px;
    right: 170px;
  }
}
</style>