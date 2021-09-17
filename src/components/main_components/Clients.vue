<template>
  <div id="clients">
    <div class="container-fluid">
      <div class="row align-items-center justify-content-evenly">
        <div class="col-auto">
          <img src="@/assets/img/client-1-2x.png" alt="AvantGarde" />
        </div>
        <div class="col-auto">
          <img src="@/assets/img/client-9-2x.png" alt="Fastlane" />
        </div>
        <div class="col-auto">
          <img src="@/assets/img/client-7-2x.png" alt="Ron Jones" />
        </div>
        <div class="col-auto">
          <img src="@/assets/img/client-3-2x.png" alt="Chippy's" />
        </div>
        <div class="col-auto">
          <img src="@/assets/img/client-4-2x.png" alt="Bullseye" />
        </div>
        <div class="col-auto">
          <img src="@/assets/img/client-5-2x.png" alt="Mighty Furnitures" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Clients",
};
</script>

<style scoped lang="scss">
img {
  cursor: pointer;
}
</style>