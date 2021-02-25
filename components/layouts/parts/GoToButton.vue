<template>
  <div class="text-center">
    <v-btn rounded :to="path" nuxt>
      go to {{ name }}
    </v-btn>
  </div>
</template>
<script>
export default {
  props: ["path", "name"],
};
</script>

<style>
</style>