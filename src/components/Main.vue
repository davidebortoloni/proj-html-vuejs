<template>
  <main>
    <Hero class="distancing" />
    <Services class="distancing" />
    <OurMission class="distancing" />
    <OurProjects class="distancing" />
    <Testimonials class="distancing" />
    <News class="distancing" />
    <CallsToAction />
    <Clients class="distancing" />
  </main>
</template>

<script>
// Importazione componenti
import Hero from "./main_components/Hero.vue";
import Services from "./main_components/Services.vue";
import OurMission from "./main_components/OurMission.vue";
import OurProjects from "./main_components/OurProjects.vue";
import Testimonials from "./main_components/Testimonials.vue";
import News from "./main_components/News.vue";
import CallsToAction from "./main_components/CallsToAction.vue";
import Clients from "./main_components/Clients.vue";

export default {
  name: "Main",
  // Registrazione componenti
  components: {
    Hero,
    Services,
    OurMission,
    OurProjects,
    Testimonials,
    News,
    CallsToAction,
    Clients,
  },
};
</script>
