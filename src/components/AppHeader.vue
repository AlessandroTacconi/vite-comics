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
    <div>
      <AppLogo />
      <AppNavBar />
    </div>
  </header>
</template>

<style scoped>
header {
  background-color: white;
}

div {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
