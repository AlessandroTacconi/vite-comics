<script>
import AppCurrentSeries from './AppCurrentSeries.vue';

export default {
  name: 'AppBlack',
  components: {
    AppCurrentSeries,
  },
};
</script>

<template>
  <div>
    <jumbotron>
      <img src="/img/jumbotron.jpg" alt="" />
    </jumbotron>
    <AppCurrentSeries />
  </div>
</template>

<style scoped>
jumbotron {
  img {
    max-width: 100vw;
    display: block;
  }
}
</style>
