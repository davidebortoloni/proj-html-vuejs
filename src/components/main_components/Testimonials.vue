<template>
  <div id="testimonials">
    <div
      class="
        content
        h-100
        text-center
        d-flex
        flex-column
        align-items-center
        justify-content-center
      "
    >
      <fa class="text-main icon" :icon="['fas', 'quote-left']" />
      <p class="fst-italic my-5">
        When it comes to barbequing, there are two main schools of thought for
        the techniques that you can use. Freshly scrambled eggs with applewood
        smoked bacon - are amazing!
      </p>
      <div class="client my-4">
        <div class="client-img my-3">
          <img
            src="@/assets/img/businesswoman-analysing-document-P8WSNMC-1024x820.jpg"
            alt="Client"
          />
        </div>
        <div class="client-name text-main">LISSA DURBIN</div>
        <div>Client</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Testimonials",
};
</script>

<style scoped lang="scss">
#testimonials {
  height: 850px;
  background-image: url("../../assets/img/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg");
  background-size: cover;
  .content {
    background-color: rgba(45, 45, 45, 0.9);
    padding: 0 400px;
    .icon {
      font-size: 50px;
    }
    p {
      font-size: 27px;
      color: rgb(184, 184, 184);
    }
    .client {
      font-family: "Quicksand", sans-serif;
      font-weight: 500;
      font-size: 20px;
      color: rgb(184, 184, 184);
      .client-img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        overflow: hidden;
        border: 5px solid white;
        display: inline-block;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          border: none;
        }
      }
      .client-name {
        font-size: 25px;
        font-weight: 500;
      }
    }
  }
}
</style>