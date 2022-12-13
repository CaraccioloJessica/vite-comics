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
  min-height: 70px;
  background-color: $blue_dc;
  padding: 20px 0;

  .container {
    min-height: 70px;
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;

    .buy_info {
      display: flex;
      align-items: center;
      padding: 10px;

      img {
        height: 40px;
        width: 40px;
        object-fit: contain;
        margin-right: 10px;
      }

      a {
        color: #fff;
        font-size: 0.7rem;
      }
    }
  }
}
</style>