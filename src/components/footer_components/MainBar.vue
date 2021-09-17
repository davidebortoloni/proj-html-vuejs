<template>
  <div id="main-bottom-bar" class="container-fluid">
    <div class="row">
      <div class="col-3 p-4">
        <a class="d-block mb-3" href="#"
          ><img src="@/assets/img/cropped-Group-39-2x.png" alt="Phlox logo"
        /></a>
        <p>
          While the lovely valley teems with vapour around me, and the meridian
          sun strikes the upper surface of the impenetrable foliage of my
          trees.While the lovely valley teems with vapour around me.
        </p>
      </div>
      <div class="col-3 p-4">
        <h3>QUICk LINKS</h3>
        <Divider />
        <ul>
          <li v-for="link in quickLinks" :key="link.id">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
      <div class="col-3 p-4">
        <h3>CONTACT</h3>
        <Divider />
        <ul>
          <li class="mb-4">
            Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, TX 76051
          </li>
          <li class="mb-4">info@yourdomain.com</li>
          <li class="mb-4">+99 (0) 101 0000 888</li>
        </ul>
      </div>
      <div class="col-3 p-4">
        <h3>LOCATION ON MAP</h3>
        <Divider />
        <img class="img-fluid" src="@/assets/img/map.png" alt="map" />
      </div>
    </div>
  </div>
</template>

<script>
import Divider from "../_generals/Divider.vue";

export default {
  name: "MainBar",
  data() {
    return {
      quickLinks: [
        {
          id: 1,
          text: "Careers",
          url: "#",
        },
        {
          id: 2,
          text: "News",
          url: "#",
        },
        {
          id: 3,
          text: "Terms of use",
          url: "#",
        },
        {
          id: 4,
          text: "Privacy Projects",
          url: "#",
        },
        {
          id: 5,
          text: "About",
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
  components: {
    Divider,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";
#main-bottom-bar {
  margin-bottom: 100px;
  h3 {
    font-size: 23px;
    font-weight: 700;
  }
  ul {
    list-style-type: none;
    padding: 0;
    a {
      color: $thirdColor;
      text-decoration: none;
      &:hover {
        color: $mainColor;
      }
    }
  }
}
</style>