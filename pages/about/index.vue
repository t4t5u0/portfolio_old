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
        <p>Deep Learning 園児neer</p>
      </div>
      <div class="dashed-box" id="history"><p>2000年生まれ。函館商業高等学校情報処理科を卒業後、公立はこだて未来大学に入学。現在は、同大学複雑系コースに在籍している。</p></div>
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
      <div id="sns"></div>
      <div id="go-to-home"><n-link to="/"> Go to Home</n-link></div>
    </div>
    <TheFooter />
  </div>
</template>

<script>
export default {};
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
  height: 150px;
  margin-right: auto;
  margin-left: auto;
  margin-top: 30px;
  margin-bottom: 30px;
  text-align: center;
}

#face-img > img {
  width: 150px;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
}

#profile {
  width: 90%;
  /* height: 150px; */
  margin: auto;
  text-align: center;
  font-size: 20px;
}

#history {
  /* height: 200px; */
  width: 90%;
  margin: auto;
  margin-left: auto;
  margin-top: 10px;
  margin-bottom: 10px;
  
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

#go-to-home{
  margin-left:10px ;
}
</style>