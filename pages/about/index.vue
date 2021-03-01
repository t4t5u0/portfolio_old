<template>
  <div>
    <TopHeader />
    <h2>Profile</h2>
    <h2>Skills</h2>
    <v-list>
      <v-list-item v-for="skill in skills" :key="skill">
        <v-list-item-avatar
          ><v-icon>{{ skill.image }}</v-icon></v-list-item-avatar
        >
        <v-list-item-content>
          <v-list-item-title>{{ skill.name }}</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <h2>Social</h2>
    <v-container>
      <v-row justify="senter" justify-lg="senter" justify-xl="senter">
        <v-col
          cols="12"
          xs="12"
          sm="6"
          md="6"
          lg="6"
          xl="4"
          v-for="item in social"
          :key="item.id"
        >
          <v-card>
            <v-avatar tile size="128">
              <img :src="item.image" />
            </v-avatar>
            <v-card-title>{{ item.title }}</v-card-title>
          </v-card>
          <!-- <CardContent :title="item.title" /> -->
        </v-col>
      </v-row>
    </v-container>
    <TheFooter />
  </div>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        {
          name: "Python",
          image: "mdi-language-python",
        },
        {
          name: "Go",
          image: "mdi-language-go",
        },
        {
          name: "Nuxt",
          image: "mdi-nuxt",
        },
        {
          name: "Rust",
          image: "mdi-language-rust",
        },
        {
          name: "Git",
          image: "mdi-git",
        },
        {
          name: "GitHub",
          image: "mdi-github",
        },
        {
          name: "Docker",
          image: "mdi-docker",
        },
        {
          name: "Discord Bot",
          image: "mdi-discord",
        },
        {
          name: "Deep Learning",
          image: "mdi-brain",
        },
      ],
      social: [
        {
          title: "GitHub",
          image:
            "https://placehold.jp/000000/ffffff/150x150.png?text=GitHub%20icon%0A150x150",
          link: "https://github.com/t4t5u0",
        },
        {
          title: "Qiita",
          image:
            "https://placehold.jp/6cf567/ffffff/150x150.png?text=Qiita%20icon%0A150x150",
          link: "https://qiita.com/t4t5u0",
        },
        {
          title: "Zenn",
          image:
            "https://placehold.jp/60c0ff/ffffff/150x150.png?text=Zenn%20icon%0A150x150",
          link: "https://zenn.dev/t4t5u0",
        },
        {
          title: "Twitter",
          image:
            "https://placehold.jp/54c0ff/ffffff/150x150.png?text=Twitter%20icon%0A150x150",
          link: "https://twitter.com/i4mwh4ti4m",
        },
        {
          title: "Discord",
          image:
            "https://placehold.jp/7289da/ffffff/150x150.png?text=Discord%20icon%0A150x150",
          link: "https://discord.com/invite/t4t5u0#4649",
        },
        {
          title: "Spotify",
          image:
            "https://placehold.jp/6cf567/ffffff/150x150.png?text=Spotify%20icon%0A150x150",
          link:
            "https://open.spotify.com/user/rezvsvhniitx1fypvambvmui7?si=q09eyhkaTn-rJpBTq2LSEw",
        },
      ],
    };
  },
};
</script>

<style>
</style>