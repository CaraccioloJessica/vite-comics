<script>
export default {

}
</script>

<template>
  <div class="card">
    <img
      src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
      alt="">
    <h3>TITOLO</h3>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

.card {
  width: calc(100% / 6);
  height: 160px;
  margin: 20px;

  img {
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: top;
  }

  h3 {
    color: #fff;
    font-size: 0.6rem;
    margin: 10px 0;
  }
}
</style>