<script>
export default {
  name: 'Navbar',
  data() {
    return {
      barraNavigazione: [
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
      <li v-for="li in barraNavigazione">
        {{ li.nome }}
        <div class="prova"></div>
      </li>
    </ul>
  </nav>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

ul {
  display: flex;
  gap: 35px;
  text-transform: uppercase;
  margin: 50px 0;
  li {
    list-style: none;
    position: relative;
    &:hover {
      color: $blue;
      cursor: pointer;
    }
  }
}
</style>
