<template>
  <div class="footer__links">
    <h3>
      {{ title }}
    </h3>
    <ul>
      <li v-for="(link,i) in links" :key="i">
        <a href="#">{{link.text}}</a>
      </li>
    </ul>
  </div>  
</template>

<script>
export default {
  props: {
    title: String,
    links: Array,
  }
}
</script>

<style scoped lang="scss">
h3 {
  text-transform: uppercase;
  padding: 1rem 0;
}

li {
  color: #999b94;
  line-height: 20px;
  font-size: 12px;
}
</style>