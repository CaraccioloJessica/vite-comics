<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <footer>
    <div class="blue_bar">
      <div class="container">
        <div class="buy_info">
          <img src="/img/buy-comics-digital-comics.png" alt="">
          <a href="#">
            DIGITAL COMICS
          </a>
        </div>
        <div class="buy_info">
          <img src="/img/buy-comics-digital-comics.png" alt="">
          <a href="#">
            DIGITAL COMICS
          </a>
        </div>
        <div class="buy_info">
          <img src="/img/buy-comics-digital-comics.png" alt="">
          <a href="#">
            DIGITAL COMICS
          </a>
        </div>
        <div class="buy_info">
          <img src="/img/buy-comics-digital-comics.png" alt="">
          <a href="#">
            DIGITAL COMICS
          </a>
        </div>
        <div class="buy_info">
          <img src="/img/buy-comics-digital-comics.png" alt="">
          <a href="#">
            DIGITAL COMICS
          </a>
        </div>
      </div>
    </div>
  </footer>

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