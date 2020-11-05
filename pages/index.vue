<template>
  <div>
    <div class="mainpage">
      <TheHeader />
      <div class="dashed-box" id="work">work1</div>
      <div class="dashed-box" id="work">work2</div>
      <div class="dashed-box" id="link-more-works">
        <n-link to="/works"> more Works</n-link>
      </div>
      <div class="dashed-box">
      <div class="dashed-box" id="face-img">
        <img src="https://placehold.jp/150x150.png?text=face" alt="face" />
      </div>
      <div class="dashed-box" id="profile">
        <!-- <p>山本竜生 | Ryuki Yamamoto</p> -->
        <p>たつお | t4t5u0</p>
        <p>Deep Learning 園児near</p>
        <p><n-link to="/works"> more information</n-link></p>
      </div>
      </div>
      <!-- <h1> This is Main </h1>
      <p><n-link to="/about">Go to About</n-link></p>
      <p><n-link to="/works">Go to Works</n-link></p>
      <Container />
      <Container />
      <Container /> -->
    </div>
    <TheFooter />
  </div>
</template>

<script>
export default {};
</script>

<style>
.mainpage {
  min-height: calc(100vh - 100px);
}

div {
  margin: 0%;
  padding: 0%;
  /* display: flex;
  flex-direction: column; */
}

.dashed-box {
  border: dashed 1px;
  box-sizing: border-box;
  margin-left: 5%;
  margin-right: 5%;
  margin-top: 10px;
  margin-bottom: 10px;
}

#work {
  /* margin: auto; */

  width: 90vw;
  height: 75vw;
}

#link-more-works{
  display: flex;
  height: 100px;
  text-align: center;
  font-size: 20px;
  vertical-align: center;
  justify-content: center;
  align-items: center;
  font-size: 30px;
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
  /* margin: auto; */
}

#profile {
  width: 90%;
  /* height: 150px; */
  margin: auto;
  margin-bottom: 30px;
  text-align: center;
  font-size: min(calc(100vw / 20), 40px);
}

</style>