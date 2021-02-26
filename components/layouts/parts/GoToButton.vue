<template>
  <v-btn :to="path" nuxt outlined width="150" class="scoped"> go to {{ name }} </v-btn>
</template>
<script>
export default {
  props: ["path", "name"],
};
</script>

<style>
.scoped {
  /* margin: auto; */
  text-align: center;
}
</style>