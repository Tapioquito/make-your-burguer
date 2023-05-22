<template>
  <v-container
    fluid
    class="main-container d-flex flex-column justify-center align-center"
  >
    <Banner />
    <h1>Monte seu burguer</h1>
    <BurguerForm />
  </v-container>
</template>

<script>
import Banner from "@/components/Banner.vue";
import BurguerForm from "@/components/BurguerForm.vue";
export default {
  name: "HomeView",
  components: { Banner, BurguerForm },
};
</script>
<style scoped>
.main-container {
  /*width: 100vw;*/
}
</style>
