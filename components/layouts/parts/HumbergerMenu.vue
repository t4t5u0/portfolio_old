<template>
  <div>
    <div id="app">
      <div class="hamburger_btn" v-on:click="isActive = !isActive">
        <span
          class="line line_01"
          v-bind:class="{ btn_line01: isActive }"
        ></span>
        <span
          class="line line_02"
          v-bind:class="{ btn_line02: isActive }"
        ></span>
        <span
          class="line line_03"
          v-bind:class="{ btn_line03: isActive }"
        ></span>
      </div>
    </div>
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
export default {
  data: () => ({ isActive: false }),
};
</script>


<style>
/*ボタン*/
.hamburger_btn {
  position: fixed; /*常に最上部に表示したいので固定*/
  top: 0;
  right: 0;
  width: 70px;
  height: 72px;
  cursor: pointer;
  z-index: 50;
}

.hamburger_btn .line {
  position: absolute;
  top: 0;
  left: 20px;
  width: 32px;
  height: 2px;
  background: #333333;
  text-align: center;
}

.hamburger_btn .line_01 {
  top: 16px;
  transition: 0.4s ease;
}
.hamburger_btn .line_02 {
  top: 26px;
  transition: 0.4s ease;
}
.hamburger_btn .line_03 {
  top: 36px;
  transition: 0.4s ease;
}

.btn_line01 {
  transform: translateY(10px) rotate(-45deg);
  transition: 0.4s ease;
}
.btn_line02 {
  transition: 0.4s ease;
  opacity: 0;
}
.btn_line03 {
  transform: translateY(-10px) rotate(45deg);
  transition: 0.4s ease;
}

/*サイドバー*/
.menu-enter-active,
.menu-leave-active {
  transition: opacity 0.4s;
}
.menu-enter,
.menu-leave-to {
  opacity: 0;
}
.menu-leave,
.menu-enter-to {
  opacity: 1;
}

.menu li {
  list-style: none;
  line-height: 1;
  padding: 1rem;
}


.menu {
  background-color: rgba(197, 197, 197, 0.8);
  z-index: 30;
  padding-top: 2rem ;
  position: fixed;
  width: 100vw;
  height: 100vh;
  top: 0;
  right: 0;
}

.menu a {
  color: rgb(66, 66, 66);
  text-decoration: none;
  font-size: 1.2rem;
  padding: 0 2rem;
}
.menu ul {
  margin: 1rem;
  padding: 0;
}
</style>