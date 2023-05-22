<template>
  <div class="d-flex justify start align-center" id="main-banner">
    <h1 color="grey-lighten-5" class="text-center py-10 px-5 bg-grey-darken-4">
      Make your Burguer
    </h1>
  </div>
</template>
<script>
export default {
  name: "BannerVue",
};
</script>

<style scoped>
#main-banner {
  background-image: url("../../public/img/burger.jpg");
  background-position: 0 -250px;
  background-size: cover;
  height: 500px;
  width: 99vw;
}
#main-banner h1 {
  font-size: 60px;
}
</style>
