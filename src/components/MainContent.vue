<template>
  <main class="main__content">
    <div class="container">
      <h1>
        Content goes here
      </h1>
    </div>
  </main>
  
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">

  @import '../style/variables';

  .main__content {
    background-color: black;
    .container {
      color:$color-white;
      padding: 2.5rem 0;
    }
  }
</style>