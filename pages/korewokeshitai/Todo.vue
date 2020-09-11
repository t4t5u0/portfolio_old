<template>
  <ul>
    <li v-for="item in items" :key="item.message">
      {{ item.message }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { message: "リンクからボタンにする" },
        { message: "フラットデザインに変更" }
      ]
    };
  }
};
</script>

<style>
body {
  background-image: none;
  background-color: aliceblue;
}
</style>
