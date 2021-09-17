<template>
  <!-- Menù principale -->
  <nav id="top-nav">
    <div class="container">
      <div class="row justify-content-between align-items-center py-4">
        <div class="col-auto">
          <a href="#"
            ><img src="@/assets/img/cropped-Group-39-2x.png" alt="Phlox logo"
          /></a>
        </div>
        <div class="col-auto">
          <!-- Links menù -->
          <ul class="m-0">
            <li
              class="px-3"
              :class="link.active ? 'active' : ''"
              v-for="link in links"
              :key="link.id"
            >
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col-auto">
          <!-- Bottone del carrello -->
          <button class="button btn-standard">Purchase</button>
          <!-- Bottone per la ricerca -->
          <fa class="ms-4 clickable text-main" :icon="['fas', 'search']" />
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "MainBar",
  // Dati necessari per la navigazione
  data() {
    return {
      // Array con voci del menù
      links: [
        {
          id: 1,
          text: "Home",
          url: "#",
          active: true,
        },
        {
          id: 2,
          text: "About",
          url: "#",
          active: false,
        },
        {
          id: 3,
          text: "Services",
          url: "#",
          active: false,
        },
        {
          id: 4,
          text: "Showcase",
          url: "#",
          active: false,
        },
        {
          id: 5,
          text: "Blog",
          url: "#",
          active: false,
        },
        {
          id: 6,
          text: "Contact",
          url: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
// Importazione variabili
@import "../../assets/scss/_vars.scss";

// Stilizzazione lista voci del menù
ul {
  list-style-type: none;
  font-size: 14px;
  li {
    display: inline-block;
    text-transform: uppercase;
    font-family: "Quicksand", sans-serif;
    font-weight: 500;
    a {
      color: $thirdColor;
      text-decoration: none;
      &:hover {
        color: $sixthColor;
      }
    }
    &.active {
      font-weight: 600;
    }
  }
}
</style>
