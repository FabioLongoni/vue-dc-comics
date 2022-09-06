<template>
  <article class="card">
    <img :src="thumb" alt="">
    <h3>{{ series }}</h3>
  </article>
</template>

<script>
export default {
  props: {
    thumb: String,
    series: String,
  }
}
</script>

<style scoped lang="scss">

  @import '../style/variables';
  .card {
    font-size:$font-size-upper;
    text-transform: uppercase;
    cursor: pointer;
    img {
      width: 200px;
      aspect-ratio: 1;
      object-fit: cover;
      object-position: top;
      margin-bottom: 1rem;
    }
  }
</style>