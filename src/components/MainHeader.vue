<template>
  <header>
    <div class="container">
      <img src="../assets/dc-logo.png" alt="">
      
      <ul class="nav-bar-header">
        <li class="active list-item"><a href="#">characters</a></li>
        <li class="list-item"><a href="#">comics</a></li>
        <li class="list-item"><a href="#">movies</a></li>
        <li class="list-item"><a href="#">tv</a></li>
        <li class="list-item"><a href="#">movies</a></li>
        <li class="list-item"><a href="#">collectibles</a></li>
        <li class="list-item"><a href="#">videos</a></li>
        <li class="list-item"><a href="#">fans</a></li>
        <li class="list-item"><a href="#">news</a></li>
        <li class="list-item"><a href="#">shop</a></li>
      </ul>
      
    </div>
  </header>
  
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">

  @import '../style/variables.scss';


  .container {
    display: flex;
    justify-content: space-between;
    padding: 1rem 0;

    .list-item {
      line-height: 100%;
      text-transform: uppercase;
      font-size: $font-size-upper;

      &.active, &:hover {
        color: $bg-light-blue;
        border-bottom: 2px solid $bg-light-blue;
      }
    }

    img {
      width: 60px;
    }

    .nav-bar-header {
      display:flex;
      gap: 1rem;
      align-items:center;
    }
  }
</style>  
  
