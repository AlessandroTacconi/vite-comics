<script>
import AppLeftFooter from './AppLeftFooter.vue';
import AppRightFooter from './AppRightFooter.vue';
import AppTopFooter from './AppTopFooter.vue';
export default {
  name: 'Footer',
  components: {
    AppLeftFooter,
    AppRightFooter,
  },
};
</script>

<template>
  <footer>
    <AppLeftFooter />
    <AppRightFooter />
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  text-transform: uppercase;
  justify-content: space-between;
  align-items: center;
  padding: 30px 0;
  background-color: #303030;
  z-index: 2;
}
</style>
