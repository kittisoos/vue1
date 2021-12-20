<template>
  <v-app>
    <Home></Home>
    <HouseWorks></HouseWorks>
  </v-app>
</template>

<script>
import Home from './components/Home';
import HouseWorks from "./components/HouseWorks";

export default {
  name: 'App',

  components: {
    HouseWorks,
    Home
  },

  data: () => ({
    //
  }),
};
</script>
