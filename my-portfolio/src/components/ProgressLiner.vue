<template>
  <v-content>
    <div class="display-2 pa-5">기술 스택</div>
    <v-row class="px-8 mt-3"
      >아래 값들은 자바스크립트를 100으로 한 상대적인 값임</v-row
    >
    <v-row class="pa-6">
      <v-col>
        JavaScript
        <v-progress-linear
          color="red lighten-2"
          rounded
          value="100"
        ></v-progress-linear>
        100%
      </v-col>
      <v-col>
        C99
        <v-progress-linear
          color="blue lighten-2"
          rounded
          value="80"
        ></v-progress-linear>
        80%
      </v-col>
      <v-col>
        Java
        <v-progress-linear
          color="brown lighten-2"
          rounded
          value="60"
        ></v-progress-linear>
        60%
      </v-col>
    </v-row>
    <v-row class="pa-6">
      <v-col>
        TypeScript
        <v-progress-linear
          color="deep-purple lighten-2"
          rounded
          value="70"
        ></v-progress-linear>
        70%
      </v-col>
      <v-col>
        C#
        <v-progress-linear
          color="orange lighten-2"
          rounded
          value="50"
        ></v-progress-linear>
        50%
      </v-col>
      <v-col>
        Kotlin
        <v-progress-linear
          color="cyan lighten-2"
          rounded
          value="20"
        ></v-progress-linear>
        20%
      </v-col>
    </v-row>
  </v-content>
</template>
<script>
export default {};
</script>
