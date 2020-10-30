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
  /* flex: 1; */
  display: flex;
  margin: 0%;
  padding: 0%;
  border: dashed 1px;
  box-sizing: border-box;
  background-color: lightgray;
  text-align: center;

  /* top: 40px; */
  /* position: absolute; */
}

#text{
  flex: 1;
}

#hmenu{
  /* flex: 1;  */
  margin: auto;
}
</style>