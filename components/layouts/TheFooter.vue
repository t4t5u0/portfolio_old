<template>
  <div>
    <div id="footer-height"></div>
    <footer><p id="footer-text">@2020 Ryuki Yamamoto</p></footer>
  </div>
</template>

<script>
export default {};
</script>

<style>
body {
  margin: 0px;
  /* min-height: calc(100vh - 100px); */
}


footer {
  /* display: flex; */
  /* flex-direction: column; */
  margin: 0%;
  padding: 0%;
  border: dashed 1px;
  background-color: lightgray;
  box-sizing: border-box;
  width: 100%;
  height: 100px;
  /* position: absolute; */
  /* position: fixed; */
  position: relative;
  /* margin-top: auto; */
  bottom: 0px;
}

/* #footer-height{
  background-color:#333333 ;
  content: "";
  display: block;
  height: 100px;
  width: 100%;
  padding-top: 100px;
} */

#footer-text {
  /* display: block; */
  /* padding: 20px; */
  text-align: center;
  margin: auto;
  vertical-align: -webkit-baseline-middle;
  /* color: yellow; */
}
</style>
