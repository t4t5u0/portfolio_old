// Qiita や Zenn に投稿した記事を挿入する
// 箱を4つ、go-to-buttonを1つ
// スマホ4*1
// PC版は2*2

<template>
  <div>
    <h2 class="scoped2">Posts</h2>
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
        <GoToButton :path="'/posts'" name="Posts" />
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
.scoped2{
  text-align: center;
  margin: 20px 0 20px 0;
}
</style>