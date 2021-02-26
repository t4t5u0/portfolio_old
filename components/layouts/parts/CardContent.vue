<template>
  <v-card outlined hover tile height="300" max-width="500" class=tmp>
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
#tmp{
  margin: auto;
}
</style>