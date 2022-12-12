<script>
export default {
  data() {
    return {

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
          <li>
            <a href="#">
              Link
            </a>
          </li>
          <li>
            <a href="#">
              Link
            </a>
          </li>
          <li>
            <a href="#">
              Link
            </a>
          </li>
          <li>
            <a href="#">
              Link
            </a>
          </li>
        </ul>
      </nav>
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

    ul {
      list-style: none;

      li {
        display: inline-block;
        padding: 1rem;
        font-weight: 600;

        a {
          color: $gray_dc;
          font-size: 0.8rem;
        }
      }
    }
  }
}
</style>