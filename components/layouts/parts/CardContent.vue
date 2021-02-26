<template>
  <v-card outlined hover tile  height="300">
    <v-card-title>{{ title }}</v-card-title>
  </v-card>
</template>

<script>
export default {
  props: {
    title: String,
  },
};
</script>

<style>
</style>