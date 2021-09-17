<template>
  <div id="our-projects">
    <div class="container-fluid">
      <div class="row align-items-center mb-3">
        <div class="col-6">
          <Divider />
          <h2>
            Our recent
            <span class="text-main">web designs</span>
            & some examples of past
            <span class="text-main">projects</span>
          </h2>
          <Divider />
        </div>
        <div class="col-6 align-self-end pb-5">
          <p>
            Far far away, behind the word mountains, far from the countries
            Vokalia and Consonantia, there live the blind texts. Separated they
            live in Bookmarksgrove right at the coast of the Semantics, a large
            language ocean. Separated they live in Bookmarksgrove.
          </p>
        </div>
      </div>
      <div class="row align-items-center g-1 p-2">
        <div class="col-3" v-for="project in projects" :key="project.id">
          <div class="project">
            <img
              :src="getImgUrl(project.imgUrl)"
              :alt="project.name"
              class="img-fluid"
            />
            <div class="overlay"></div>
            <div class="content h-100 p-3">
              <div class="h-100 d-flex flex-column justify-content-end p-3">
                <h5>{{ project.name }}</h5>
                <div>
                  <span
                    v-for="(tag, index) in project.tag"
                    :key="index"
                    class="tag"
                    :class="index + 1 < project.tag.length ? 'dot' : ''"
                  >
                    {{ tag }}
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="text-center">
        <button class="button btn-standard">Read More</button>
      </div>
    </div>
  </div>
</template>

<script>
import Divider from "../_generals/Divider.vue";

export default {
  name: "OurProjects",
  data() {
    return {
      projects: [
        {
          id: 1,
          name: "The Basket of Flowers",
          tag: ["Branding", "Marketing"],
          imgUrl: "ina-soulis-227104-unsplash-1024x1024.jpg",
        },
        {
          id: 2,
          name: "A Famous Ferris Wheel",
          tag: ["Marketing"],
          imgUrl: "sunisa-misa-531163-unsplash-1024x1024.jpg",
        },
        {
          id: 3,
          name: "Complementary Colors",
          tag: ["Branding", "Marketing"],
          imgUrl: "355H-1024x1024.jpg",
        },
        {
          id: 4,
          name: "Business Prestige",
          tag: ["Branding"],
          imgUrl: "photo-1448932252197-d19750584e56-1024x1024.jpg",
        },
        {
          id: 5,
          name: "Colorful Origami Boats",
          tag: ["Branding", "Marketing"],
          imgUrl: "business-competition-PB366D8-1024x1024.jpg",
        },
        {
          id: 6,
          name: "Modern Couch",
          tag: ["Marketing"],
          imgUrl: "cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg",
        },
        {
          id: 7,
          name: "Hot Air Balloons",
          tag: ["Branding", "Marketing"],
          imgUrl: "aa9a4539-PQGJ7HU-1024x1024.jpg",
        },
        {
          id: 8,
          name: "Make Difference",
          tag: ["Branding"],
          imgUrl: "cody-davis-253928-unsplash-1024x1024.jpg",
        },
      ],
    };
  },
  methods: {
    getImgUrl(endPoint) {
      return require(`@/assets/img/${endPoint}`);
    },
  },
  components: {
    Divider,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";

#our-projects {
  .project {
    position: relative;
    border-radius: 5px;
    overflow: hidden;
    cursor: pointer;
    color: $fifthColor;
    .content {
      display: none;
      .tag {
        text-transform: uppercase;
        font-size: 17px;
        &.dot::after {
          content: "\00B7";
          margin: 0 10px;
        }
      }
    }
    .overlay {
      width: 100%;
      height: 100%;
      display: none;
    }
    &:hover {
      transform: scale(1.1);
      z-index: 1;
      .content {
        display: block;
        position: absolute;
        top: 0;
        left: 0;
      }
      .overlay {
        position: absolute;
        top: 0;
        left: 0;
        display: block;
        background: linear-gradient(45deg, $secondaryColor, $mainColor);
        opacity: 0.8;
      }
    }
  }
  button {
    margin-top: 120px;
  }
}
</style>