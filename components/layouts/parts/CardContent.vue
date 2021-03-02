<template>
  <v-card tile height="300" max-width="500" class="scoped" color="#f5f6fb">
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
.scoped {
  margin: auto;
}
</style>

