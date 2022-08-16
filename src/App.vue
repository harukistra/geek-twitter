<template>
<div>

  <!-- <div class="nav__bar">
    <router-link to="/" class="nav__logo nav__link">GeekTwitter</router-link>
    <div class="nav__items">
      <router-link to="/about" class="nav__item nav_link">About</router-link>
      <router-link to="/my-page" class="nav__item nav_link">MyPage</router-link>
    </div>
    <router-view />

  </div> -->
  <NavBar />
  <router-view />
</div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
export default {
  components: {
    NavBar,
}
}
</script>

<style>
* {
  box-sizing: border-box;
}
body {
  margin: 0;
}
.nav__bar {
  height: 50px;
  display: flex;
  justify-content: space-between;
  align-items: stretch;
  background-color: black;
}
.nav__link {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  color: #eee;
  text-decoration: none;
}
.nav__link:visited {
  color: #eee;
}
.nav__link:hover {
  font-weight: bold;
  color: #fff;
}
.nav__logo {
  width: 130px;
}
.nav__items {
  display: flex;
}
.nav_item {
  width: 100px;
  border-left: 1px solid #eee;
}
</style>
