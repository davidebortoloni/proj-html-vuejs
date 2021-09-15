<template>
  <div class="container">
    <div class="row justify-content-between align-items-center py-4">
      <div class="col-auto">
        <a href="#"
          ><img src="@/assets/img/cropped-Group-39-2x.png" alt="Phlox logo"
        /></a>
      </div>
      <div class="col-auto">
        <ul class="m-0">
          <li class="px-3" v-for="link in links" :key="link.id">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
      <div class="col-auto">
        <button class="btn-standard">Purchase</button>
        <fa class="ms-4 clickable text-main" :icon="['fas', 'search']" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainBar",
  data() {
    return {
      links: [
        {
          id: 1,
          text: "Home",
          url: "#",
        },
        {
          id: 2,
          text: "About",
          url: "#",
        },
        {
          id: 3,
          text: "Services",
          url: "#",
        },
        {
          id: 4,
          text: "Showcase",
          url: "#",
        },
        {
          id: 5,
          text: "Blog",
          url: "#",
        },
        {
          id: 6,
          text: "Contact",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";

ul {
  list-style-type: none;
  li {
    display: inline-block;
    text-transform: uppercase;
    a {
      color: #444444;
      text-decoration: none;
      &:hover {
        color: $mainColor;
      }
    }
  }
}
</style>
