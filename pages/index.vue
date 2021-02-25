<template>
  <div>
    <div class="mainpage">
      <TheHeader />
      <TopAbout />
      <TopWorks />
      <TopPosts />
      <TopHistory />
      <GoToButton :path="'/about'" name="About"></GoToButton>
      <GoToButton :path="'/'" name="Home"></GoToButton>
    </div>
    <TheFooter />
  </div>
</template>

<script>
import GoToButton from "../components/layouts/parts/GoToButton.vue";
export default {
  components: { GoToButton },
};
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

#link-more-works {
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