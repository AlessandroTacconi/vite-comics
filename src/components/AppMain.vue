<script>
import AppBlue from './AppBlue.vue';
import AppBlack from './AppBlack.vue';

export default {
  name: 'Main',
  components: {
    AppBlue,
    AppBlack,
  },
};
</script>

<template>
  <main>
    <AppBlack />
    <AppBlue />
  </main>
</template>
