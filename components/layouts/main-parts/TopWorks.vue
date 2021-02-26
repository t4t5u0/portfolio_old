// 
// スマホ4*1
// PC版は2*2

<template>
  <div>
    <h2>Works</h2>
    <v-container>
      <v-row justify="senter">
        <v-col
          cols="12"
          xs="12"
          sm="6"
          md="6"
          lg="6"
          xl="6"
          v-for="title in Titles"
          :key="title"
        >
          <CardContent :title="title" />
        </v-col>
        <v-col cols="1">
          <GoToButton :path="'/works'" name="Works" />
        </v-col>
      </v-row>
    </v-container>
    <!-- <GoToButton :path="'/works'" name="Works" /> -->
  </div>
</template>

<script>
import GoToButton from "../parts/GoToButton.vue";
export default {
  data: () => ({
    Titles: ["Hoge", "Fuga", "Piyo", "Zura"],
  }),
  components: { GoToButton },
};
</script>

<style>
</style>