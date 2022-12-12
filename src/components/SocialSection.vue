<script>
export default {
  data() {
    return {

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
        <img src="" alt="">
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
      h4 {
        color: $blue_dc;
      }
    }
  }
}
</style>