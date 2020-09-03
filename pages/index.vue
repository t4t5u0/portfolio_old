<template>
  <div class="my-body">
    <div class="my-header">
    </div>
    <div class="container">
      <div class="main-text">
        <p>工事中</p>
      </div>
      <br />
      <div class="twitter-link">
          連絡先：<a href="https://twitter.com/i4mwh4ti4m" target="_blank">twitter</a>
      </div>
    </div>
    <div class="my-fooder">
      <!-- <br /> -->
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
body {
  margin: 0%;
  /* height: %; */
  background-color: yellow;
}

.container {
  margin: 0 auto;
  margin-top: -5em;
  margin-bottom: -10em;
  /* min-height: calc(100vh-15em); */
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  /* background-color: #ffe81c; */
}

.my-header {
  width: 100%;
  /* top: 20%; */
  height: 5em;
  background: repeating-linear-gradient(
    135deg,
    yellow 0px,
    yellow 25px,
    black 0px,
    black 50px
  );
}

.my-fooder {
  width: 100%;
  /* bottom: -10em; */
  height: 10em;
  background: repeating-linear-gradient(
    135deg,
    yellow 0px,
    yellow 25px,
    black 0px,
    black 50px
  );
}

.main-text {
  font-family: "ヒラギノ角ゴ ProN W3", "Hiragino Kaku Gothic ProN", "メイリオ",
    "Meiryo", "verdana", sans-serif;
  font-size: 10em;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.twitter-link{
  font-size: 5em;
  margin: 100px;
}
/* .header {
  width: 100%;
  top: 20%;
  background: repeating-linear-gradient(135deg, yellow, yellow, 5px, black);
} */
</style>
