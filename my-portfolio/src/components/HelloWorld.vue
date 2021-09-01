<template>
  <v-row class="display-2 pa-3 mt-3">
    <v-col
      v-for="n in 5"
      :key="n"
      class="d-flex justify-space-around mb-6"
      cols="4"
    >
      <v-img
        v-bind:src="require(`../assets/img/logo/${n}.png`)"
        :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
        aspect-ratio="1"
        contain
        class="grey lighten-2"
      >
        <template v-slot:placeholder>
          <v-row class="fill-height ma-0" align="center" justify="center">
            <v-progress-circular
              indeterminate
              color="grey lighten-5"
            ></v-progress-circular>
          </v-row>
        </template>
      </v-img>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "HelloWorld",

  data() {
    return {};
  },
};
</script>
