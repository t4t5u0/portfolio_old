// 箱を4つ。go-to-buttonを1つ
// 時系列データなので、PC版の表示でも
// 2列で表示しない


<template>
  <div>
    <h2>History</h2>
    <v-container>
      <v-row justify="senter" justify-lg="senter" justify-xl="senter">
        <v-col
          cols="12"
          xs="12"
          sm="6"
          md="6"
          lg="6"
          xl="3"
          v-for="title in Titles"
          :key="title"
        >
          <CardContent :title="title" />
        </v-col>
        <GoToButton :path="'/history'" name="History" />
      </v-row>
    </v-container>
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

<style scoped>
h2 {
  text-align: center;
  margin: 20px 0 20px 0;
}
</style>