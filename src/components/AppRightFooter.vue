<script>
export default {
  name: 'Footer Right',
  data() {
    return {
      listaFooterRight: [
        {
          nome: 'Facebook',
          link: '#',
          target: '_self',
          img: '/img/footer-facebook.png',
        },
        {
          nome: 'Twitter',
          link: '#',
          target: '_self',
          img: '/img/footer-twitter.png',
        },
        {
          nome: 'Youtube',
          link: '#',
          target: '_self',
          img: '/img/footer-youtube.png',
        },
        {
          nome: 'Pinterest',
          link: '#',
          target: '_self',
          img: '/img/footer-pinterest.png',
        },
        {
          nome: 'Periscope',
          link: '#',
          target: '_self',
          img: '/img/footer-periscope.png',
        },
      ],
    };
  },
};
</script>

<template>
  <div>
    <div>Follow us</div>
    <ul>
      <li v-for="li in listaFooterRight">
        <img :src="li.img" alt="{{ li.nome }}" />
      </li>
    </ul>
  </div>
</template>

<style scoped>
div {
  display: flex;
  align-items: center;
  gap: 30px;
  color: #0282f9;
}

li {
  list-style: none;
}

ul {
  display: flex;
  gap: 10px;
}
</style>
