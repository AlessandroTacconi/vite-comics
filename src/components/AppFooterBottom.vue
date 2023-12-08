<script>
import AppLeftFooter from './AppLeftFooter.vue';
import AppRightFooter from './AppRightFooter.vue';

export default {
  name: 'Footer bottom',
  components: {
    AppLeftFooter,
    AppRightFooter,
  },
};
</script>

<template>
  <div class="background">
    <div class="container">
      <AppLeftFooter />
      <AppRightFooter />
    </div>
  </div>
</template>

<style scoped>
.background {
  text-transform: uppercase;
  padding: 30px 0;
  background-color: #303030;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
