<template>
  <div id="header">
    <header>
      <p id="text">header</p>
      <div id="hmenu">
        <HumbergerMenu />
      </div>
    </header>
  </div>
</template>

<script>
export default {};
</script>

<style>
header {
  /* display: flex; */
  margin: 0%;
  padding: 0%;
  /* height: 100px; */
  border: dashed 1px;
  box-sizing: border-box;
  background-color: lightgray;
  text-align: center;
}

#text {
  /* flex: 1; */
}

#hmenu {
  /* flex: 1;  */
  /* margin: auto; 
  position: fixed; /*常に最上部に表示したいので固定
  top: 10px;
  right: 0px;
  width: 100px;
  height: 100px;
  cursor: pointer;
  z-index: 50;  */
}
</style>