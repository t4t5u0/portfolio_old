<template>
  <div>
    <div class="mainpage">
      <TheHeader />
      <h1> This is Main </h1>
      <p><n-link to="/about">Go to About</n-link></p>
      <p><n-link to="/works">Go to Works</n-link></p>
      <Container />
      <Container />
      <Container />
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
</style>