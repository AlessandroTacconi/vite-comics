<script>
import AppTopFooter from './AppTopFooter.vue';
import AppFooterBottom from './AppFooterBottom.vue';

export default {
  name: 'Footer',
  components: {
    AppTopFooter,
    AppFooterBottom,
  },
};
</script>

<template>
  <footer>
    <AppTopFooter />
    <AppFooterBottom />
  </footer>
</template>

<style scoped></style>
