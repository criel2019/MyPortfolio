<template>
  <v-carousel v-model="model" >
    <v-carousel-item @mouseover="overlay = true" @mouseleave="overlay =false" v-for="(item, i) in items" :src="item.src" :key="i">
      <v-row justify="center" >
        <v-overlay
          :absolute="absolute"
          :opacity="opacity"
          :value="overlay"
          class="fill-height display-2 blue--text"
          align="center"
          justify="center"
          color="#F5F5F5"
        >
          {{context[i]}}
        </v-overlay>
      </v-row>
      </v-row>
    </v-carousel-item>
  </v-carousel>
</template>
<script>
export default {
  data: () => ({
    model: 0,
    absolute: true,
    context: ["Web", "Android", "Unity"],
    opacity: 1,
    overlay: false,
    items: [
      {
        src: require("../assets/img/advist_main.png"),
      },
      {
        src: require("../assets/img/mobile.png"),
      },
      {
        src: require("../assets/img/unity.jpg"),
      },
    ],
    colors: ["primary", "secondary", "yellow darken-2", "red", "orange"],
  }),
};
</script>
