<template>
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
    <v-spacer></v-spacer>
    <v-app-bar-nav-icon> </v-app-bar-nav-icon>
  </v-app-bar>
</template>

<script>
export default {};
</script>

<style>
</style>