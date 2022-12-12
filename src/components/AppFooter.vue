<script>

export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <div class="background_image">
    <div class="container">
      <div class="menu_section">
        <ul>
          <h4>DC COMICS</h4>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
        </ul>

        <ul>
          <h4>DC COMICS</h4>
          <li>ddddd</li>
          <li>ddddd</li>
        </ul>

        <ul>
          <h4>DC COMICS</h4>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
        </ul>

        <ul>
          <h4>DC COMICS</h4>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
          <li>ddddd</li>
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
  height: 280px;
  background-repeat: no-repeat;
  overflow: hidden;

  .container {
    display: flex;
    justify-content: space-between;

    .menu_section {
      display: flex;

      h4 {
        color: #fff;
        padding: 2rem 2.5rem 1rem 0;
      }

      li {
        color: #959595;
        padding: 0.2rem 0;
        font-size: 0.8rem;
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