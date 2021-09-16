<template>
  <div>
    <Hero />
    <Services />
  </div>
</template>

<script>
import Hero from "./main_components/Hero.vue";
import Services from "./main_components/Services.vue";

export default {
  name: "Main",
  components: {
    Hero,
    Services,
  },
};
</script>
