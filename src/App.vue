<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppTopFooter from './components/AppTopFooter.vue';
export default {
  components: {
    AppHeader,
    AppMain,
    AppTopFooter,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppTopFooter />
  <AppFooter />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
</style>
