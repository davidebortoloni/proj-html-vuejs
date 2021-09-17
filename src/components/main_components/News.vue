<template>
  <div id="news">
    <div class="container-fluid">
      <div class="row">
        <div class="col-12 d-flex flex-column align-items-center">
          <h2>Latest News & Our <span class="text-main">Blog</span></h2>
          <Divider />
        </div>
        <div class="col-12">
          <div class="row">
            <div class="col-4" v-for="article in articles" :key="article.id">
              <div class="content">
                <div class="cover">
                  <img
                    :src="getImgUrl(article.imgUrl)"
                    :alt="article.name"
                    class="img-fluid"
                  />
                </div>
                <div class="info">
                  <div class="details mb-2">
                    {{ article.date }} &bull; by {{ article.author }}
                  </div>
                  <div class="title">
                    <span class="dot me-1">&#9679;</span>
                    {{ article.name }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-12 d-flex justify-content-center">
          <button class="button btn-reverse">View All Post</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Divider from "../_generals/Divider.vue";

export default {
  name: "News",
  data() {
    return {
      articles: [
        {
          id: 1,
          name: "Marketing Ideas",
          date: "May 24, 2018",
          author: "Alex",
          imgUrl:
            "serious-businesswoman-with-documents-talking-on-P9Q6LX6-1024.jpg",
        },
        {
          id: 2,
          name: "Rest During Working Hours",
          date: "May 24, 2018",
          author: "Alex",
          imgUrl: "Businessman-at-the-desk-in-his-office-resting--1024x768.jpg",
        },
        {
          id: 3,
          name: "Develop Your Startup Idea",
          date: "May 24, 2018",
          author: "Alex",
          imgUrl: "simple-home-office-with-tree-PBXRXYB-large-1024x768.jpg",
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

.content {
  width: 100%;
  position: relative;
  cursor: pointer;
  .cover {
    border-radius: 10px;
    overflow: hidden;
  }
  .info {
    background-color: white;
    padding: 40px 20px;
    width: 80%;
    position: absolute;
    bottom: -50px;
    left: 50%;
    transform: translate(-50%);
    border-radius: 10px;
    font-family: "Quicksand", sans-serif;
    .details {
      padding-left: 25px;
      color: $sixthColor;
      font-size: 14px;
      font-weight: 500;
    }
    .title {
      .dot {
        color: $mainColor;
      }
      font-size: 23px;
      font-weight: 700;
    }
  }
  &:hover {
    .info {
      background: linear-gradient(90deg, $secondaryColor, $mainColor);
      .details,
      .title,
      .dot {
        color: white;
      }
    }
  }
}
button {
  margin-top: 100px;
}
</style>