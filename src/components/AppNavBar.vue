<script>
export default {
  name: 'Navbar',
  data() {
    return {
      barranavigazione: [
        { nome: 'Characters', link: '#', target: '_self' },
        { nome: 'Comic', link: '#', target: '_self' },
        { nome: 'Movies', link: '#', target: '_self' },
        { nome: 'TV', link: '#', target: '_self' },
        { nome: 'Games', link: '#', target: '_self' },
        { nome: 'Collectibles', link: '#', target: '_self' },
        { nome: 'Videos', link: '#', target: '_self' },
        { nome: 'Fans', link: '#', target: '_self' },
        { nome: 'News', link: '#', target: '_self' },
        { nome: 'Shop', link: '#', target: '_self' },
      ],
    };
  },
};
</script>

<template>
  <nav>
    <ul>
      <li v-for="li in barranavigazione">{{ li.nome }}</li>
    </ul>
  </nav>
</template>

<style scoped>
li {
  list-style: none;
}

ul {
  display: flex;
  gap: 35px;
  text-transform: uppercase;
}
</style>
