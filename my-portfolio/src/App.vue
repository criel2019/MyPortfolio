<template>
  <v-app>
    <v-main>
      <Parallax />
      <ProgressLiner />
      <Carousel />
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Parallax from "./components/Parallax";
import Carousel from "./components/Carousel";
import ProgressLiner from "./components/ProgressLiner";

export default {
  name: "App",

  components: {
    HelloWorld,
    Parallax,
    Carousel,
    ProgressLiner,
  },

  data: () => ({
    //
  }),
};
</script>
