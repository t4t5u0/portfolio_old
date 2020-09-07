<template>
  <div class="my-body">
    <LHeader />
    <div class="container">
      <div id="item1" class="main-text">
        <p>工事中</p>
      </div>
      <div id="item2" class="twitter-link">連絡先：<a href="https://twitter.com/i4mwh4ti4m" target="_blank"
          >twitter</a
        >
      </div>
    </div>
    <LFooter />
  </div>
</template>

<script>
import LHeader from "../components/layouts/Header";
import LFooter from "../components/layouts/Footer";

export default {
  components: { LFooter, LHeader }
};
</script>

<style>
body {
  margin: 0%;
  /* height: %; */
  background-color: yellow;
}

.container {
  display: grid;
  gap: 10px;
  /* grid-auto-rows: minmax(100px, auto); */
  /* grid-template-columns: repeat(2, 1fr); */
  grid-template-columns: repeat(auto-fit, minmax(200px, 500px));
  grid-template-rows: repeat(auto-fit, minmax(200px, 1fr));
  /* min-height: calc(100vh-15em); */
  /* min-height: 100vh; */
  /* min-width: 1fr; */
  /* align-items: center; */
  /* text-align: center; */
}

#item1{
  /* grid-row: 1;
  grid-column: 1; */
  text-align: center;
  border-radius: 10px;
  background-color: rgba(230, 230, 230, 0.35);
}

#item2{
  /* grid-row: 1;
  grid-column: 2; */
  text-align: center;
  border-radius: 10px;
  background-color: rgba(230, 230, 230, 0.35);
}

.main-text {
  font-family: "ヒラギノ角ゴ ProN W3", "Hiragino Kaku Gothic ProN", "メイリオ",
    "Meiryo", "verdana", sans-serif;
  font-size: 10em;
  margin: 10px;
}

.twitter-link {
  font-size: 5em;
  margin: 10px;
}
</style>
