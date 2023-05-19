<template>
  <v-app>
    <NavBar :logo="logo_src" :alt="app_name" /> <RouterView></RouterView
    ><Footer></Footer
  ></v-app>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: { NavBar, Footer },
  data() {
    return { logo_src: "/img/logo.png", app_name: "Make Your Burguer" };
  },
};
</script>

<style>
* {
  font-family: Arial, Helvetica, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.main-container {
  height: 900px;
  min-height: 250px;
  color: #222;
}
</style>
