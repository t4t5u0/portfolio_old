// 簡単なプロフィールと、go-to-button を1つ
// テーブルの中でv-forを回すのが良さそう
// 
<template>
  <div>
    <h2 class="centering">About</h2>
    <v-simple-table>
      <template v-slot:default>
        <!-- <thead>
          <tr>
            <th>First</th>
            <th>Second</th>
          </tr>
        </thead> -->
        <tbody>
          <tr v-for="item in content1" :key="item.key">
            <td>{{ item.key }}</td>
            <td>{{ item.value }}</td>
          </tr>
          <!-- linkつき -->
          <tr v-for="item in content2" :key="item.key">
            <td>{{ item.key }}</td>
            <td>
              <a :href="item.link" target="_blank" class="no-margin">{{
                item.value
              }}</a>
            </td>
          </tr>
          <!-- skills -->
          <tr v-for="item in content3" :key="item.key">
            <td>{{ item.key }}</td>
            <td>
              <ul v-for="lang in item.value" :key="lang.id">
                <li>{{ lang }}</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
  </div>
</template>

<script>
export default {
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
.no-margin {
  margin: 0 auto;
}

.centering{
  text-align: center;
  padding: 20px;
}
</style>
