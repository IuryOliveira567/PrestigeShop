<template>
  <div class="main-layout">
    <header>
      <NavBar/>
    </header>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import NavBar from './components/NavBar.vue';

export default defineComponent({
  name: 'App',
  components: {
    NavBar
  }
});
</script>

<style lang="scss">
</style>
