<script>
import AppLogo from './AppLogo.vue';
import AppNavBar from './AppNavBar.vue';
export default {
  name: 'Header',
  components: {
    AppLogo,
    AppNavBar,
  },
};
</script>

<template>
  <header class="container">
    <AppLogo />
    <AppNavBar />
  </header>
</template>

<style scoped>
header {
  background-color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 0;
}
</style>
