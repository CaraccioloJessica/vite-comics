<script>
export default {
  data() {
    return {
      socials: [
        {
          img: './img/footer-facebook.png',
          url: '#',
          alt: 'Facebook'
        },
        {
          img: './img/footer-twitter.png',
          url: '#',
          alt: 'Twitter'
        },
        {
          img: './img/footer-youtube.png',
          url: '#',
          alt: 'Youtube'
        },
        {
          img: './img/footer-pinterest.png',
          url: '#',
          alt: 'Pinterest'
        },
        {
          img: './img/footer-periscope.png',
          url: '#',
          alt: 'Periscope'
        },
      ]
    }
  }
}
</script>

<template>
  <div class="gray_bar">
    <div class="container">
      <button>
        <a href="#">
          SIGN-UP NOW!
        </a>
      </button>

      <div class="socials">
        <h4>
          FOLLOW US
        </h4>
        <a v-for="social in socials" :href="social.url">
          <img :src="social.img" :alt="social.alt">
        </a>
      </div>
    </div>
  </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

.gray_bar {
  height: 80px;
  background-color: $gray_dc;

  .container {
    height: inherit;
    display: flex;
    align-items: center;
    justify-content: space-between;

    button {
      background-color: $gray_dc;
      padding: 0.6rem;
      border: 2px solid $blue_dc;

      a {
        color: #fff;
        font-size: 0.7rem;
      }
    }

    .socials {
      display: flex;
      align-items: center;

      h4 {
        color: $blue_dc;
        margin-right: 1rem;
      }

      img {
        height: 1.6rem;
        margin: 0 0.4rem;
      }
    }
  }
}
</style>