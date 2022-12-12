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
    display: flex;
    justify-content: space-between;

    .menu_section {
      height: 300px;
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;

      ul {
        padding-right: 2.5rem;

        h4 {
          color: #fff;
          padding: 0.9rem 0 0.6rem 0;
        }

        li a {
          color: #959595;
          padding-bottom: 0.3rem;
          font-size: 0.7rem;
        }
      }
    }

    .big_logo {
      width: 400px;
      position: relative;

      img {
        overflow: hidden;
        position: absolute;
        top: -65px;
      }
    }
  }
}
</style>