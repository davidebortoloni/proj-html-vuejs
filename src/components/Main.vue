<template>
  <div>
    <Hero class="distancing" />
    <Services class="distancing" />
    <OurMission class="distancing" />
    <OurProjects class="distancing" />
    <Testimonials class="distancing" />
    <News class="distancing" />
  </div>
</template>

<script>
import Hero from "./main_components/Hero.vue";
import Services from "./main_components/Services.vue";
import OurMission from "./main_components/OurMission.vue";
import OurProjects from "./main_components/OurProjects.vue";
import Testimonials from "./main_components/Testimonials.vue";
import News from "./main_components/News.vue";

export default {
  name: "Main",
  components: {
    Hero,
    Services,
    OurMission,
    OurProjects,
    Testimonials,
    News,
  },
};
</script>
