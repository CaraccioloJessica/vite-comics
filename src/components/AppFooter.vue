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
        wwww
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

    .menu_section {}

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