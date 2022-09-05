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
      <section class="footer__second__section">
        <div class="container">
          <div class="ul__wrapper">
            <div>
              <h3>
                dc comics
              </h3>
              <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>New</li>
              </ul>
              <h3>
                shop
              </h3>
              <ul>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
              </ul>
            </div>
            <div>
              <h3>
                Dc
              </h3>
              <ul>
                <li>Terms Of Use</li>
                <li>Privacy policy(New)</li>
                <li>Ad choises</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>Subsccription</li>
                <li>Talent Workshops</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
              </ul>
            </div>
            <div>
              <h3>
                Sites
              </h3>
              <ul>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
              </ul>
            </div>
          </div>
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
    background-color: $light-blue;

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
          color: $color-white;
          text-transform: uppercase;
          font-size: $font-size-upper;

          img {
            width: 40px;
          } 
        }
      }
    }
  }
  .footer__second__section {
    color: $color-white;
    background-color: BLACK;

    .container {
      padding: 2rem 0;

      .ul__wrapper {
        display: flex;
        gap: 2rem;

        h3 {
          text-transform: uppercase;
          padding: 1rem 0;
        }

        li {
          color: #65d781;
          line-height: 20px;
          font-size: 12px;
        }

      }
    }
  }
</style>