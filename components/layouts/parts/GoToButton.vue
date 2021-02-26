<template>
  <v-btn :to="path" nuxt outlined width="150"> go to {{ name }} </v-btn>
</template>
<script>
export default {
  props: ["path", "name"],
};
</script>

<style>
#hoge {
  margin: auto;
}
</style>