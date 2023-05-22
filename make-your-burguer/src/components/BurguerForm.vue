<template>
  <v-form
    fast-fail
    v-model="valid"
    id="burguer-form"
    class="d-flex flex-column justify-center align-center"
  >
    <v-text-field
      v-model="name"
      label="Nome"
      required
      class="label"
    ></v-text-field>
    <v-select
      class="label"
      v-model="select"
      :rules="[(v) => !!v || 'Item is required']"
      label="Pão"
      required
    ></v-select>
    <v-select
      class="label"
      v-model="select"
      :rules="[(v) => !!v || 'Item is required']"
      label="Carne"
      required
    ></v-select>
    <v-checkbox
      class="label"
      v-model="checkbox"
      label="Escolha os opcionais:"
      required
    ></v-checkbox>
    <v-btn>Criar meu burguer</v-btn>
  </v-form>
</template>
<script>
export default {
  name: "BurguerForm",
  data() {
    return {
      valid: true,
      name: "",
      nameRules: [
        (v) => !!v || "Nome é obrigatório",
        (v) =>
          (v && v.length <= 10) || "Nome deve possuir pelo menos 10 caracteres",
      ],
      select: null,
      paes: ["Brioche", "Seda", "Três Queijos"],
    };
  },
};
</script>
<style scoped>
#burguer-form {
  max-width: 400px;
  margin: 0 auto;
}
.label {
  width: 300px;
}
</style>
