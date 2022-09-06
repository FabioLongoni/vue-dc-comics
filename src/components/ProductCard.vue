<template>
  <article class="card">
    <img :src="thumb" alt="">
    <div>{{ series }}</div>
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
    font-weight: lighter;
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