<template>
  <div>
    <div class="aboutpage">
      <TheHeader />
      <div class="dashed-box" id="face-img">
        <img src="https://placehold.jp/150x150.png?text=face" alt="face" />
      </div>
      <div class="dashed-box" id="profile">
        <!-- <p>山本竜生 | Ryuki Yamamoto</p> -->
        <p>たつお | t4t5u0</p>
        <p>Deep Learning 園児near</p>
      </div>
      <div class="dashed-box" id="history">
        <p>
          2000年生まれ。函館商業高等学校情報処理科を卒業後、公立はこだて未来大学に入学。現在は、同大学複雑系コースに在籍している。
        </p>
      </div>
      <div class="dashed-box" id="info">
        <div id="inline-box">
          <ul id="list-intersting">
            興味
            <li>声質変換</li>
            <li>深層学習</li>
          </ul>
          <ul id="list-language">
            言語
            <li>Python</li>
            <li>Go</li>
            <li>Nuxt</li>
          </ul>
        </div>
        <ul id="list-like">
          好き
          <li>プログラミング</li>
          <li>スノーバーガー</li>
          <li>喫茶店に通う</li>
          <li>邦ロック</li>
        </ul>
      </div>
      <div id="sns" class="dashed-box">
        <ul>
          <li v-for="item in object" :key="item.title" class="sns-image-link">
            <a :href="item.link" target="_blank"><img :src="item.image" :alt="item.title" /></a>
          </li>
        </ul>
      </div>
      <div id="go-to-home"><n-link to="/"> Go to Home</n-link></div>
    </div>
    <TheFooter />
  </div>
</template>

<script>
export default {
  data() {
    return {
      object: [
        {
          title: "Twitter",
          image:
            "https://placehold.jp/54c0ff/ffffff/150x150.png?text=Twitter%20icon%0A150x150",
          link: "https://twitter.com/i4mwh4ti4m",
        },
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
      ],
    };
  },
};
</script>

<style>
.aboutpage {
  min-height: calc(100vh - 100px);
}

.dashed-box {
  border: dashed 1px;
  box-sizing: border-box;
}

#face-img {
  width: 90%;
  /* height: 150px; */
  margin-right: auto;
  margin-left: auto;
  margin-top: 30px;
  margin-bottom: 30px;
  text-align: center;
  /* vertical-align: baseline; */
}

#face-img > img {
  /* width: 150px; */
  /* height: 150px; */
  width: 50vw;
  height: 50vw;
  max-width: 400px;
  max-height: 400px;
  object-fit: cover;
  border-radius: 50%;
}

#profile {
  width: 90%;
  /* height: 150px; */
  margin: auto;
  text-align: center;
  font-size: min(calc(100vw / 20), 40px);
}

#history {
  /* height: 200px; */
  width: 90%;
  margin: auto;
  margin-left: auto;
  margin-top: 10px;
  margin-bottom: 10px;
  font-size: min(calc(100vw / 32), 28px); /* メディアクエリ使いなさい */
}

#history > p {
  width: 80%;
  margin: auto;
  text-align: center;
}

#info {
  display: flex;
  flex-direction: column;
  width: 90%;
  /* height: 150px; */
  margin-right: auto;
  margin-left: auto;
  margin-top: 10px;
  margin-bottom: 50px;
}

#inline-box {
  display: flex;
}

#list-intersting {
  flex: 1;
}

#list-language {
  flex: 1;
}

#list-like {
  flex: 1;
}

#sns {
  width: 90%;
  margin: auto;
}

#sns > ul {
  list-style: none;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

#sns > li{
  margin: 0px;
  padding: 0px;
}

.sns-image-link {
  flex: 1;
  /* margin: 10px; */
  padding: 0;
  text-align: center;
}

.sns-image-link > a {
  width: 0;
  height: 0;
}

.sns-image-link > a > img {
  border-radius: 50%;
  width: min(20vw, 150px);
  vertical-align: bottom;
}

#go-to-home {
  margin-left: 5%;
  font-size: 20px;
}
</style>