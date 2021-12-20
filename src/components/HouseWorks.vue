<template>
  <v-card>
    <v-checkbox
        v-model="porszivozas"
        :label="'Porszívózás'"
    ></v-checkbox>
    <v-checkbox
        v-model="felmosas"
        :label="'Felmosás'"
    ></v-checkbox>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      porszivozas: false,
      felmosas: false
    }
  },
}
</script>

<style>
v-card {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>