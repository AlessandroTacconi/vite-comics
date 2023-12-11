<script>
export default { props: ['image', 'title'] };
</script>
<template>
  <div class="comic">
    <img :src="image" :alt="title" />
    <div>{{ title }}</div>
  </div>
</template>
