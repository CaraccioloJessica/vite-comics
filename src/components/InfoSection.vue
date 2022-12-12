<script>
export default {
  data() {
    return {
      shop: [
        {
          img: '/img/buy-comics-digital-comics.png',
          text: 'DIGITAL COMICS',
          url: '#'
        },
        {
          img: '/img/buy-comics-merchandise.png',
          text: 'DC MERCHANDISE',
          url: '#'
        },
        {
          img: '/img/buy-comics-subscriptions.png',
          text: 'SUBCRIPTION',
          url: '#'
        },
        {
          img: '/img/buy-comics-shop-locator.png',
          text: 'COMIC SHOP LOCATOR',
          url: '#'
        },
        {
          img: '/img/buy-dc-power-visa.svg',
          text: 'DC POWER VISA',
          url: '#'
        }
      ]
    }
  }
}
</script>

<template>
  <div class="blue_bar">
    <div class="container">
      <div class="buy_info" v-for="link in shop">
        <img :src="link.img" :alt="link.text">
        <a :href="link.url">
          {{ link.text }}
        </a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

.blue_bar {
  // Margini da rimuovere quando ci sarà il main
  margin-top: 100px;
  height: 120px;
  background-color: $blue_dc;

  .container {
    display: flex;
    justify-content: center;

    .buy_info {
      height: 120px;
      display: flex;
      align-items: center;

      img {
        height: 40px;
        width: 55px;
        object-fit: contain;
        padding-right: 0.7rem;
      }


      a {
        color: #fff;
        font-size: 0.7rem;
        padding-right: 3.5rem;
      }
    }
  }
}
</style>