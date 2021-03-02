<template>
  <div>
    <TopHeader />
    <h2 class="tac">Works</h2>
    <v-container>
      <v-row justify="senter">
        <v-col cols="12" xs="12" sm="6" md="6" lg="6" xl="3">
          <v-card tile height="500" max-width="500" color="#f5f6fb">
            <v-img
              height="250"
              src="https://media.discordapp.net/attachments/422717592407375872/816285228451758110/20210302092318_cropped.png"
            ></v-img>
            <v-card-title>Sort Riddle Bot</v-card-title>
            <v-card-text
              >ソートなぞなぞというゲームをDiscord
              Botにしました。ソートなぞなぞとは、文字列を文字コード順に並べ替え、並べ替える前の文字列を推測する遊びです。</v-card-text
            >
            <v-chip-group column active-class="white--text">
              <v-chip disabled color="#ffd900" text-color="#00f">Python</v-chip>
              <v-chip disabled color="#7289da" text-color="#111"
                >Discord Bot</v-chip
              >
            </v-chip-group>

            <v-btn
              rounded
              href="http://github.com/t4t5u0/sort-riddle-v2"
              target="_blank"
              >view on GitHub</v-btn
            >
            <v-btn
              rounded
              href="./works/pages/sort_riddle"
              target="_blank"
              >more</v-btn
            >
          </v-card>
        </v-col>
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
        <GoToButton :path="'/'" name="Home" />
      </v-row>
    </v-container>
    <TheFooter />
  </div>
</template>

<script>
export default {
  data: () => ({
    Titles: ["Hoge", "Fuga", "Piyo", "Zura", "Hoge", "Fuga", "Piyo", "Zura"],
  }),
};
</script>

<style scoped>
.tac {
  text-align: center;
}
</style>