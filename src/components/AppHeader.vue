<script>
export default {
  data() {
    return {
      links: [
        {
          text: 'CHARACTERS',
          url: '#',
          current: false,
        },
        {
          text: 'COMICS',
          url: '#',
          current: true,
        },
        {
          text: 'MOVIES',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'GAMES',
          url: '#',
          current: false,
        },
        {
          text: 'COLLECTIBLES',
          url: '#',
          current: false,
        },
        {
          text: 'VIDEOS',
          url: '#',
          current: false,
        },
        {
          text: 'FANS',
          url: '#',
          current: false,
        },
        {
          text: 'NEWS',
          url: '#',
          current: false,
        },
        {
          text: 'SHOP',
          url: '#',
          current: false,
        },
      ]
    }
  }
}

</script>

<template>
  <header>
    <div class="container">
      <a href="#">
        <img src="/img/dc-logo.png" alt="DC">
      </a>

      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :class="{ active: link.current }" :href="link.url">
              {{ link.text }}
            </a>
          </li>
        </ul>
      </nav>
    </div>

    <div class="jumbo">
      <img src="/img/jumbotron.jpg" alt="">
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

header {
  background-color: #fff;

  .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 90px;

    img {
      transform: scale(0.55);
    }

    li {
      display: inline-block;
      padding: 0.6rem;
      font-weight: 600;

      a {
        color: $gray_dc;
        font-size: 0.7rem;

        &:hover,
        &.active {
          color: $blue_dc;
          border-bottom: 3px solid $blue_dc;
          padding-bottom: 2.1rem;
        }
      }
    }
  }

  .jumbo {
    max-height: 280px;
    overflow: hidden;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}
</style>