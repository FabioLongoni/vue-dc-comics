<template>
    <footer>
      <section class="footer__first__section">
        <div class="small__container">
          <ul>
            <li :key="i" v-for="(card,i) in listCards">
              <img :src="card.image" alt="">
              <a href="#">{{card.text}}</a>
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
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">New</a></li>
              </ul>
              <h3>
                shop
              </h3>
              <ul>
                <li><a href="#">Shop DC</a></li>
                <li><a href="#">Shop DC Collectibles</a></li>
              </ul>
            </div>
            <div>
              <h3>
                Dc
              </h3>
              <ul>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Privacy policy(New)</a></li>
                <li><a href="#">Ad choises</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscription</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
              </ul>
            </div>
            <div>
              <h3>
                Sites
              </h3>
              <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">AD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
              </ul>
            </div>
          </div>
          <img src="../assets/dc-logo-bg.png" alt="">
        </div>
      </section>
      <section class="footer__third__section">
        <div class="container">
          <div class="sign__up__button">
            <a href="#">sign-up now</a>
          </div>
          <div class="footer__media">
            <span>follow us</span>
            <div class="footer__icon">
              <a href="#"><img src="../assets/footer-facebook.png" alt=""></a>
              <a href="#"><img src="../assets/footer-twitter.png" alt=""></a>
              <a href="#"><img src="../assets/footer-youtube.png" alt=""></a>
              <a href="#"><img src="../assets/footer-pinterest.png" alt=""></a>
              <a href="#"><img src="../assets/footer-periscope.png" alt=""></a>
            </div>
          </div>
        </div>
      </section>
      
    </footer>
</template>

<script>



export default {
  data() { 
    return {
      listCards: [
        {
          image: require("../assets/buy-comics-digital-comics.png"),
          text: "digital comics",
        },
        {
          image: require("../assets/buy-comics-merchandise.png"),
          text: "dc merchandise",
        },
        {
          image: require("../assets/buy-comics-subscriptions.png"),
          text: "subscriptions",
        },
        {
          image: require("../assets/buy-comics-shop-locator.png"),
          text: "comic shop locator",
        },
        {
          image: require("../assets/buy-dc-power-visa.svg"),
          text: "dc power visa",
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  
  @import '../style/variables';

  .footer__first__section {
    background-color: $light-blue;
    overflow: hidden;

    .small__container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 2rem 0;

      ul {
        display: flex;
        align-items: center;
        gap: 2rem;

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
    background-image: url('../assets/footer-bg.jpg');


    .container {
      padding: 2rem 0;
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 320px;
      overflow: hidden;

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
      img {
        transform: scale(0.9,0.9);
      }
    }
  }

  .footer__third__section {
    background-color: #303030;
    padding: 2rem 0;

    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;

      .footer__media {
        display: flex;
        align-items: center;
        gap: 1.5rem;

        .footer__icon {
          display: flex;
          gap: 1rem;
        }

        span {
          color: $light-blue;
          text-transform: uppercase;
          font-weight: bold;
        }
      }
    }

    .sign__up__button {
      color: $color-white;
      text-transform: uppercase;
      font-size: 16px;
      padding: 1rem 0;

      a {
        padding: 1rem;
        border: 2px solid $light-blue;
      }
      
    }
  }
</style>