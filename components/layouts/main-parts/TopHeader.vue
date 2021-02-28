<template>
  <dev>
    <v-app-bar
      fixed
      color="#fff"
      dark
      shrink-on-scroll
      src="https://picsum.photos/1920/1080?random"
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(19,84,122,.5), rgba(128,208,199,.8)"
        ></v-img>
      </template>
      <v-app-bar-title>t4t5u0's portfolio</v-app-bar-title>
      <v-spacer />
      <HumbergerMenu />
    </v-app-bar>
    <v-sheet id="scrolling-techniques" class="overflow-y-auto" height="136" />
  </dev>
</template>

<script>
export default {};
</script>

<style>
</style>