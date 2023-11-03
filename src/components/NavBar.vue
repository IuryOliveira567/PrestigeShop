<template>
  <div class="nav-bar">
    <nav>
      <div class="mobile-menu" @click="isMobileMenu = !isMobileMenu">
        <div></div>
        <div></div>
        <div></div>
      </div>
      <div class="logo-name">
        <h3>PRESTIGE SHOP</h3>
      </div>
      <div class="shop"><i class="fa-solid fa-cart-shopping"></i></div>
    </nav>
    <ul v-if="isMobileMenu" class="nav">
      <li class="nav-item"><a class="nav-link" href="#">My Account</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Shop</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Gifts</a></li>
      <li class="nav-item"><a class="nav-link" href="#">About Us</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Contact Us</a></li>
      <li class="nav-item"><a class="nav-link" href="#">My Account</a></li>
    </ul>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'NarBar',
  data() {
    return {
      isMobileMenu: false
    }
  }
})
</script>

<style scoped lang="scss">
nav {
  display: flex;
  align-items: center;
  justify-content: space-around;
  border: 1px solid black;
}

.mobile-menu {
  border: 1px solid gray;
  width: 50px;
  border-radius: 5px;
  margin: 8px;
  cursor: pointer;
}

.mobile-menu div {
  width: 32px;
  height: 2px;
  background-color: gray;
  margin: 8px;
  border-radius: 2px;
}

.nav {
  display: block;
  background-color: gray;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  height: 80vh;
}
</style>