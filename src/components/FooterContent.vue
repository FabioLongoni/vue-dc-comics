<template>
    <footer>
      <section class="footer__first__section">
        <div class="small__container">
        <ul>
          <li>
            <img src="../assets/buy-comics-digital-comics.png" alt="">
            <a href="#">digital comics</a>
          </li>
        </ul>
      </div>
      </section>
      
    </footer>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
  
  @import '../style/variables';

  .footer__first__section {
    background-color: $bg-light-blue;

    .small__container {
      max-width: 900px;
      margin: 0 auto;
      padding: 2rem 0;

      ul {
        display: flex;
        align-items: center;
        li {
          display:flex;
          gap: 1rem;
          align-items: center;
          color: white;
          text-transform: uppercase;
          font-size: $font-size-upper;

          img {
            width: 40px;
          } 
        }
      }
    }
  }
</style>