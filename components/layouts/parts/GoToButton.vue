<template>
  <v-btn :to="path" nuxt outlined width="150" class="scoped1"> go to {{ name }} </v-btn>
</template>
<script>
export default {
  props: ["path", "name"],
};
</script>

<style>
.scoped1 {
  margin: 0 auto;
  text-align: center;
}
</style>