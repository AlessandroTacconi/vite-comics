<script>
export default {
  name: 'Blue bar',
  data() {
    return {
      listaBlu: [
        {
          nome: 'Digital Comics',
          link: '#',
          target: '_self',
          img: '/img/buy-comics-digital-comics.png',
        },
        {
          nome: 'DC Merchandise',
          link: '#',
          target: '_self',
          img: '/img/buy-comics-merchandise.png',
        },
        {
          nome: 'Subscription',
          link: '#',
          target: '_self',
          img: '/img/buy-comics-subscriptions.png',
        },
        {
          nome: 'Comic Shop Locator',
          link: '#',
          target: '_self',
          img: '/img/buy-comics-shop-locator.png',
        },
        {
          nome: 'DC Powre visa',
          link: '#',
          target: '_self',
          img: '/img/buy-dc-power-visa.svg',
        },
      ],
    };
  },
};
</script>

<template>
  <nav>
    <ul class="container">
      <li v-for="li in listaBlu">
        <div><img :src="li.img" alt="{{ li.nome }}" /></div>
        <div>{{ li.nome }}</div>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
ul {
  display: flex;
  justify-content: center;
  gap: 80px;
  color: white;
  text-transform: uppercase;
  padding: 75px;
}

li {
  display: flex;
  align-items: center;
  gap: 8px;
}

nav {
  background-color: #0282f9;
}

img {
  height: 50px;
}
</style>
