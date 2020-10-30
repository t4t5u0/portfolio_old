<template>
  <burger-button :active="isActive" @click="isActive = !isActive" />
</template>

<script>
import BurgerButton from "vue-burger-button";
export default {
  components: { BurgerButton },
  data: () => ({ isActive: false }),
};
</script>

<style src="vue-burger-button/dist/vue-burger-button.css" />