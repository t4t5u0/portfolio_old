// 簡単なプロフィールと、go-to-button を1つ
// テーブルの中でv-forを回すのが良さそう
// 
<template>
  <div>
    <h2 class="centering">About</h2>
    <v-list width="80%" class="m0a">
      <v-list-item v-for="item in content1" :key="item">
        <v-list-item-content>{{ item.key }}</v-list-item-content>
        <v-list-item-content>{{ item.value }}</v-list-item-content>
      </v-list-item>
      <v-list-item v-for="item in content2" :key="item">
        <v-list-item-content>{{ item.key }}</v-list-item-content>
        <v-list-item-content
          ><a :href="item.link"> {{ item.value }}</a></v-list-item-content
        >
      </v-list-item>
      <div v-for="item in content3" :key="item">
        <v-list-item v-for="(lang, index) in item.value" :key="lang">
          <v-list-item-content>{{
            index === 0 ? item.key : ""
          }}</v-list-item-content>
          <v-list-item-content>{{ lang }}</v-list-item-content>
        </v-list-item>
      </div>
    </v-list>
    <v-container>
      <v-row>
        <GoToButton :path="'/about'" name="About" />
      </v-row>
    </v-container>
  </div>
</template>

<script>
import GoToButton from "../parts/GoToButton.vue";
export default {
  components: { GoToButton },
  data() {
    return {
      content1: [
        {
          key: "Name",
          value: "Ryuki Yamamoto (山本 竜生)",
        },
        {
          key: "University",
          value:
            "公立はこだて未来大学 情報システム科学部 複雑系知能学科 複雑系コース",
        },
      ],
      content2: [
        {
          key: "GitHub",
          value: "t4t5u0",
          link: "https://github.com/t4t5u0",
        },
        {
          key: "Qiita",
          value: "t4t5u0",
          link: "https://qiita.com/t4t5u0",
        },
        {
          key: "Twitter",
          value: "@i4mwh4ti4m",
          link: "https://twitter.com/i4mwh4ti4m",
        },
      ],
      content3: [
        {
          key: "Skills",
          value: ["Python", "Go"],
        },
      ],
    };
  },
};
</script>

<style scoped>
.m0a {
  margin: 0 auto;
}

.centering {
  text-align: center;
  padding: 20px;
}
</style>