<template>
  <div>
    <Hero class="distancing" />
    <Services class="distancing" />
    <OurMission class="distancing" />
    <OurProjects class="distancing" />
  </div>
</template>

<script>
import Hero from "./main_components/Hero.vue";
import Services from "./main_components/Services.vue";
import OurMission from "./main_components/OurMission.vue";
import OurProjects from "./main_components/OurProjects.vue";

export default {
  name: "Main",
  components: {
    Hero,
    Services,
    OurMission,
    OurProjects,
  },
};
</script>
