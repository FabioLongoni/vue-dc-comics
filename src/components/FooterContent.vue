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
              <LinksFooter title="dc comics" :links="linksMenù1"/>
              <LinksFooter title="shop" :links="linksMenù2"/> 
            </div>     
            <div>
              <LinksFooter title="dc" :links="linksMenù3"/>
            </div>
            <div>
              <LinksFooter title="sites" :links="linksMenù4"/>
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
              <a href="#" v-for="(icon,i) in iconsList" :key="i">
                <img :src="icon.image" alt="">
              </a>
            </div>
          </div>
        </div>
      </section>
      
    </footer>
</template>

<script>
import LinksFooter from './LinksFooter.vue';

export default {
  components: {
    LinksFooter,
},
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
      ],
      linksMenù1: [
        {
          text: 'Characters',
          href: '#'
        },
        {
          text: 'Comics',
          href: '#'
        },
        {
          text: 'Movies',
          href: '#'
        },
        {
          text: 'Tv',
          href: '#'
        },
        {
          text: 'Games',
          href: '#'
        },
        {
          text: 'Videos',
          href: '#'
        },
        {
          text: 'News',
          href: '#'
        },
      ],
      linksMenù2: [
        {
          text: 'Shop DC',
          href: '#'
        },
        {
          text: 'Shop DC Collectibles',
          href: '#'
        },
      ],
      linksMenù3: [
        {
          text: 'Terms Of Use',
          href: '#'
        },
        {
          text: 'Privacy policy(New)',
          href: '#'
        },
        {
          text: 'Ad choises',
          href: '#'
        },
        {
          text: 'Advertising',
          href: '#'
        },
        {
          text: 'Games',
          href: '#'
        },
        {
          text: 'Jobs',
          href: '#'
        },
        {
          text: 'CPSC Certificates',
          href: '#'
        },
        {
          text: 'Talent Workshops',
          href: '#'
        },
        {
          text: 'Ratings',
          href: '#'
        },
        {
          text: 'Shop Help',
          href: '#'
        },
        {
          text: 'Contact Us',
          href: '#'
        },
      ],
      linksMenù4: [
        {
          text: 'DC',
          href: '#'
        },
        {
          text: 'AD Magazine',
          href: '#'
        },
        {
          text: 'DC Kids',
          href: '#'
        },
        {
          text: 'DC Universe',
          href: '#'
        },
        {
          text: 'DC Power Visa',
          href: '#'
        }
      ],
      iconsList: [
        {
          image: require("../assets/footer-facebook.png")
        },
        {
          image: require("../assets/footer-twitter.png")
        },
        {
          image: require("../assets/footer-youtube.png")          
        },
        {
          image: require("../assets/footer-pinterest.png")
        },
        {
          image: require("../assets/footer-periscope.png")
        },
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