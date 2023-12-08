<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './style/partials/variables.scss' as *;
@use './style/partials/typo.scss' as *;
@use './style/general.scss' as *;

.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>
