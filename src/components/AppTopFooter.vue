<script>
export default {
  name: 'top footer',
  data() {
    return {
      dcComics: [
        { nome: 'Characters', link: '#', target: '_self' },
        { nome: 'Comic', link: '#', target: '_self' },
        { nome: 'Movies', link: '#', target: '_self' },
        { nome: 'TV', link: '#', target: '_self' },
        { nome: 'Games', link: '#', target: '_self' },
        { nome: 'Videos', link: '#', target: '_self' },
        { nome: 'News', link: '#', target: '_self' },
      ],
      shop: [
        { nome: 'Shop DC', link: '#', target: '_self' },
        { nome: 'Shop DC Collectibles', link: '#', target: '_self' },
      ],
      dc: [
        { nome: 'Terms Of Use', link: '#', target: '_self' },
        { nome: 'Privaci Policy (New)', link: '#', target: '_self' },
        { nome: 'Ad Choice', link: '#', target: '_self' },
        { nome: 'Advertising', link: '#', target: '_self' },
        { nome: 'Jobs', link: '#', target: '_self' },
        { nome: 'Subscriptions', link: '#', target: '_self' },
        { nome: 'Talent Workshops', link: '#', target: '_self' },
        { nome: 'CPSC Certificates', link: '#', target: '_self' },
        { nome: 'Ratings', link: '#', target: '_self' },
        { nome: 'Shop Help', link: '#', target: '_self' },
        { nome: 'Contact Us', link: '#', target: '_self' },
      ],
      sites: [
        { nome: 'DC', link: '#', target: '_self' },
        { nome: 'MAD Magazine', link: '#', target: '_self' },
        { nome: 'DC Kids', link: '#', target: '_self' },
        { nome: 'DC Universe', link: '#', target: '_self' },
        { nome: 'DC Power Visa', link: '#', target: '_self' },
      ],
    };
  },
};
</script>

<template>
  <div class="top-footer">
    <div class="container">
      <div class="liste">
        <div>
          <h2 class="titolo">DC Comics</h2>
          <ul class="dc-comics">
            <li v-for="li in dcComics">{{ li.nome }}</li>
          </ul>
          <h2 class="titolo">Shop</h2>
          <ul>
            <li v-for="li in shop">{{ li.nome }}</li>
          </ul>
        </div>
        <div>
          <h2 class="titolo">DC</h2>
          <ul>
            <li v-for="li in dc">{{ li.nome }}</li>
          </ul>
        </div>
        <div>
          <h2 class="titolo">Sites</h2>
          <ul>
            <li v-for="li in sites">{{ li.nome }}</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

.top-footer {
  background-image: url('/img/footer-bg.jpg');
  background-size: cover;
}

.container {
  background-image: url('/img/dc-logo-bg.png');
  background-size: 560px;
  background-repeat: no-repeat;
  background-position: right;
}

.liste {
  display: flex;
  gap: 60px;
  padding: 45px 0;
}

ul {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

li {
  list-style: none;
  color: #959595;
}

.titolo {
  text-transform: uppercase;
  color: $white;
  margin-bottom: 25px;
}

.dc-comics {
  margin-bottom: 25px;
}
</style>
