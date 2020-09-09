<template>
  <div class="my-body">
    <!-- <LHeader /> -->
    <div class="container">
      <div id="item" class="main-text">
        <p>工事中</p>
      </div>
      <!-- <div id="item" class="twitter-link"> -->
      <div id="item" class="sacrament">
        Contact:
        <a href="https://twitter.com/i4mwh4ti4m" target="_blank">Twitter</a>
      </div>
      <div id="item" class="sacrament">hogehoge</div>
    </div>
    <!-- <LFooter /> -->
  </div>
</template>

<script>
import LHeader from "../components/layouts/Header";
import LFooter from "../components/layouts/Footer";

export default {
  components: { LFooter, LHeader },
};
</script>

<style>
body {
  margin: 0%;
  /* height: %; */
  /* background-color: yellow; */
  background-color: rgb(70, 70, 70);
  background-image: linear-gradient(
      335deg,
      rgb(0, 0, 0) 23px,
      transparent 23px
    ),
    linear-gradient(155deg, #191919 23px, transparent 23px),
    linear-gradient(335deg, #191919 23px, transparent 23px),
    linear-gradient(155deg, #191919 23px, transparent 23px);
  background-size: 58px 58px;
  background-position: 0px 2px, 4px 35px, 29px 31px, 34px 6px;
}

.container {
  display: grid;
  gap: 10px;
  /* grid-auto-rows: minmax(100px, auto); */
  /* grid-template-columns: repeat(2, 1fr); */
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-template-rows: repeat(auto-fit, minmax(200px, 1fr));
  /* min-height: calc(100vh-15em); */
  min-height: 300px;
  /* min-width: 1fr; */
  /* align-items: center; */
  /* text-align: center; */
}

#item {
  /* grid-row: 1;
  grid-column: 1; */
  /* margin :10x; */
  text-align: center;
  /* vertical-align: middle; */
  border-radius: 10px;
  background-color: rgba(88, 88, 88, 0.7);
}

/* #item1 {
  grid-row: 1;
  grid-column: 1;
  text-align: center;
  border-radius: 10px;
  background-color: rgba(230, 230, 230, 0.35);
}

#item2 {
  grid-row: 1;
  grid-column: 2;
  text-align: center;
  border-radius: 10px;
  background-color: rgba(230, 230, 230, 0.35);
} */

.main-text {
  /* font-family: "ヒラギノ角ゴ ProN W3", "Hiragino Kaku Gothic ProN", "メイリオ",
    "Meiryo", "verdana", sans-serif; */
  font-family: "M PLUS Rounded 1c", sans-serif;
  font-weight: 100;
  font-size: 4em;
  margin: 10px;
  /* color: white; */
  color: rgba(255, 255, 255, 0.6);
  text-align: center;
  vertical-align: middle;
  text-shadow: 1px 5px 4px rgba(0, 0, 0, 0.3), 0 0 2px rgba(255, 255, 255, 1),
    0 0 10px rgba(255, 255, 255, 1), 0 0 20px rgba(255, 255, 255, 1),
    0 0 30px rgba(255, 255, 255, 1), 0 0 40px #ff00de, 0 0 70px #ff00de,
    0 0 80px #ff00de, 0 0 100px #ff00de;
}

.twitter-link {
  /* font-size: 5em; */
  margin: 10px;
}

.sacrament {
  margin: 10px;
  font-family: "Sacramento", cursive;
  font-size: 4em;
  /* font-family: 'Pacifico', cursive; */
  /* font-size:80px; */
  border: none;
  color: rgba(255, 255, 255, 0.6);
  text-align: center;
  vertical-align: middle;
  text-shadow: 1px 5px 4px rgba(0, 0, 0, 0.3), 0 0 2px rgba(255, 255, 255, 1),
    0 0 10px rgba(255, 255, 255, 1), 0 0 20px rgba(255, 255, 255, 1),
    0 0 30px rgba(255, 255, 255, 1), 0 0 40px #ff00de, 0 0 70px #ff00de,
    0 0 80px #ff00de, 0 0 100px #ff00de;
}
</style>
