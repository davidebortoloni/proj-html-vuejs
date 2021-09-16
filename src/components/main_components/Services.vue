<template>
  <div id="services">
    <div class="container-fluid h-100">
      <div class="h-100 row align-items-center">
        <div class="col-5">
          <div class="content">
            <h2>
              We Are Here To Make Your
              <span class="text-main">Website</span> Look More
              <span class="text-main">Elegant</span> And Stylish!
            </h2>
            <Divider />
            <button class="button btn-standard my-3">VIEW ALL</button>
          </div>
        </div>
        <div class="col-7">
          <div class="row gy-5">
            <div
              class="col-6"
              v-for="(service, index) in services"
              :key="index"
            >
              <div class="card">
                <fa
                  :icon="[service.icon.family, service.icon.name]"
                  class="icon my-3"
                />
                <h3 class="my-3">{{ service.name }}</h3>
                <p>{{ service.text }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Divider from "../_generals/Divider.vue";

export default {
  name: "Services",
  data() {
    return {
      services: [
        {
          icon: {
            family: "fas",
            name: "tachometer-alt",
          },
          name: "Speed Optimization",
          text: "Far far away, behind the word mountains, far from the countries Vokalia Separated...",
        },
        {
          icon: {
            family: "fas",
            name: "cloud",
          },
          name: "Cloud Solutions",
          text: "Far far away, behind the word mountains, far from the countries Vokalia Separated...",
        },
        {
          icon: {
            family: "fas",
            name: "mobile-alt",
          },
          name: "Website Design",
          text: "Far far away, behind the word mountains, far from the countries Vokalia Separated...",
        },
        {
          icon: {
            family: "fas",
            name: "stopwatch",
          },
          name: "Online Marketing",
          text: "Far far away, behind the word mountains, far from the countries Vokalia Separated...",
        },
      ],
    };
  },
  components: {
    Divider,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";

h2 {
  font-weight: 600 !important;
}
.card {
  border: none;
  box-shadow: 0 0 40px -15px $sixthColor;
  padding: 40px;
  border-radius: 20px;
  cursor: pointer;
  color: $thirdColor;
  &:hover {
    background: linear-gradient(90deg, $secondaryColor, $mainColor);
    color: white;
  }
  .icon {
    font-size: 70px;
  }
}
</style>