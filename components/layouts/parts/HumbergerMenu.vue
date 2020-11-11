<template>
  <div>
    <burger-button :active="isActive" @click="isActive = !isActive">
    </burger-button>
    <transition name="menu">
      <div class="menu" v-show="isActive">
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/works">Works</a></li>
          <li><a href="/about">About</a></li>
        </ul>
      </div>
    </transition>
  </div>
</template>

<script>
import BurgerButton from "vue-burger-button";
export default {
  components: { BurgerButton },
  data: () => ({ isActive: false }),
};
</script>

<style src="vue-burger-button/dist/vue-burger-button.css" />