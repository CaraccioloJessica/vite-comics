<script>
export default {
  props: {
    details: Object
  }
}
</script>

<template>
  <div class="card">
    <img :src="details.thumb" :alt="details.series">
    <h3>{{ details.series }}</h3>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

.card {
  width: calc(140px - 20px);
  height: 120px;
  margin: 20px 10px;

  img {
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: top;
  }

  h3 {
    color: #fff;
    font-size: 0.7rem;
    margin-top: 10px;
  }
}
</style>