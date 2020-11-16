<template>
  <div>
    <div id="workspage">
      <TheHeader />
      <h1>This is Works</h1>
      <n-link to="/"> Go to Home</n-link>
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
#workspage {
  min-height: calc(100vh - 100px); 
}

h1, a{
  margin-left: 5%;
}

</style>