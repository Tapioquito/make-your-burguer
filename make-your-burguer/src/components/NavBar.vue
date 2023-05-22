<template>
  <v-app-bar class="bg-grey-darken-4">
    <v-container class="d-flex justify-end px-13 mb-0">
      <RouterLink :to="{ name: 'home' }" class="img_logo"
        ><v-img :width="25" :height="25" :src="logo" :alt="alt"></v-img
      ></RouterLink>

      <RouterLink id="golden" :to="{ name: 'home' }"><h3>Home</h3></RouterLink>

      <RouterLink id="golden" :to="{ name: 'pedidos' }"
        ><h3>Pedidos</h3></RouterLink
      >
    </v-container>
  </v-app-bar>
</template>
<script>
export default {
  name: "NavBar",
  props: ["logo", "alt"],
};
</script>
<style scoped>
#golden {
  color: #fcba03;
  text-decoration: none;
  padding: 0px 30px;
  transition: 0.5s;
}
#golden:hover {
  color: #fff;
}
.img_logo {
  margin: auto;
  margin-left: 0;
}
</style>
