<script>

export default {
  data() {
    return {
      menu: [
        {
          title: 'DC COMICS',
          links: [
            {
              text: 'Characters',
              url: '#'
            },
            {
              text: 'Comics',
              url: '#'
            },
            {
              text: 'Movies',
              url: '#'
            },
            {
              text: 'TV',
              url: '#'
            },
            {
              text: 'Games',
              url: '#'
            },
            {
              text: 'Videos',
              url: '#'
            },
            {
              text: 'News',
              url: '#'
            },
          ]
        },
        {
          title: 'SHOP',
          links: [
            {
              text: 'Shop DC',
              url: '#'
            },
            {
              text: 'Shop DC Collectibles',
              url: '#'
            },
          ]
        },
        {
          title: 'DC',
          links: [
            {
              text: 'Terms Of Use',
              url: '#'
            },
            {
              text: 'Privacy policy (New)',
              url: '#'
            },
            {
              text: 'Ad Choices',
              url: '#'
            },
            {
              text: 'Advertising',
              url: '#'
            },
            {
              text: 'Jobs',
              url: '#'
            },
            {
              text: 'Subscriptions',
              url: '#'
            },
            {
              text: 'Talent Workshops',
              url: '#'
            },
            {
              text: 'CPSC Certificates',
              url: '#'
            },
            {
              text: 'Ratings',
              url: '#'
            },
            {
              text: 'Shop Help',
              url: '#'
            },
            {
              text: 'Contact Us',
              url: '#'
            },
          ]
        },
        {
          title: 'SITES',
          links: [
            {
              text: 'DC',
              url: '#'
            },
            {
              text: 'MAD Magazine',
              url: '#'
            },
            {
              text: 'DC kids',
              url: '#'
            },
            {
              text: 'DC Universe',
              url: '#'
            },
            {
              text: 'DC Power Visa',
              url: '#'
            },
          ]
        }
      ]
    }
  }
}
</script>

<template>
  <div class="background_image">
    <div class="container">
      <div class="menu_section">
        <ul v-for="(item, index) in menu" :key="index">
          <h4>
            {{ item.title }}
          </h4>
          <li v-for="elem in item.links">
            <a :href="elem.url">
              {{ elem.text }}
            </a>
          </li>
        </ul>
      </div>

      <div class="big_logo">
        <img src="/img/dc-logo-bg.png" alt="dc-logo">
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

.background_image {
  background-image: url('./img/footer-bg.jpg');
  height: 270px;
  background-repeat: no-repeat;
  overflow: hidden;

  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;

    .menu_section {
      padding-top: 1rem;
      height: 100%;
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;

      ul {
        padding-right: 2rem;

        h4 {
          color: #fff;
          font-size: 0.9rem;
          padding: 10px 0;
        }

        li {
          display: flex;
          margin-bottom: 0.2rem;

          a {
            color: #959595;
            font-size: 0.65rem;
          }
        }
      }
    }

    .big_logo {
      width: 400px;
      height: 100%;

      img {
        overflow: hidden;
        position: relative;
        top: -4rem;
      }
    }
  }
}

@media screen and (max-width: 1100px) {
  .container {
    max-width: 90%;
  }
}

@media screen and (max-width: 788px) {
  .big_logo {
    opacity: 0.3;
  }
}
</style>