<template>
  <div>
    <div class="mainpage">
      <TheHeader />
      <Container />
      <Container />
      <Container />
      <n-link to="/about">Go to About</n-link><br />
      <n-link to="/works">Go to works</n-link>
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