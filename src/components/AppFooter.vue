<template>
  <footer class="footer">
      <div class="footer__container-top container">
          <div class="footer__menu">
              <ul class="footer__list">
                  <li>
                      <h3>dc comics</h3>
                  </li>
                  <li
                  v-for="(element, index) in firstList"
                  :key="index"
                  >
                      <a href="">{{ element.text }}</a>
                  </li>
                  
              </ul>
              <ul class="footer__list">
                  <li>
                      <h3>dc</h3>
                  </li>
                  <li
                  v-for="(element, index) in secondList"
                  :key="index"
                  >
                      <a href="">{{ element.text}}</a>
                  </li>
              </ul>
              <ul class="footer__list">
                  <li>
                      <h3>sites</h3>
                  </li>
                  <li
                  v-for="(element, index) in thirdList"
                  :key="index"
                  >
                      <a href="">{{ element.text }}</a>
                  </li>
              </ul>
              <ul class="footer__list">
                  <li>
                      <h3>shop</h3>
                  </li>
                  <li
                  v-for="(element, index) in fourthList"
                  :key="index"
                  >
                      <a href="">{{ element.text }}</a>
                  </li>
              </ul>
          </div>
          <div class="footer__logo">
              <img src="../assets/img/dc-logo-bg.png" alt="">
          </div>
      </div>
      <div class="footer__container-bottom container">
        <div class="footer__button">
            <a href="">sign-up now!</a>
        </div>
        <div class="footer__social">
            <span>follow us</span>
            <img src="../assets/img/footer-facebook.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: "AppFooter",
    data: function () {
        return {
            firstList: [
                  {
                      url: "#",
                      text: "Characters",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "Comics",
                      active: true,
                  },
                  {
                      url: "#",
                      text: "Movies",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "Tv",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "Games",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "Collectibles",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "Videos",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "Fans",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "News",
                      active: false,
                  },
                  {
                      url: "#",
                      text: "Shop",
                      active: false,
                  },
            ],
            secondList: [
                {
                    url: "#",
                    text: "Terms Of Use",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Privacy policy(New)",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Add Choises",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Advertising",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Jobs",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Subscriptions",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Talent Workshops",
                    active: false, 
                },
                {
                    url: "#",
                    text: "CPSC Certificates",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Ratings",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Shop Help",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Contacts Us",
                    active: false, 
                },
            ],
            thirdList: [
                {
                    url: "#",
                    text: "DC",
                    active: false, 
                },
                {
                    url: "#",
                    text: "MAD Magazine",
                    active: false, 
                },
                {
                    url: "#",
                    text: "DC Kids",
                    active: false, 
                },
                {
                    url: "#",
                    text: "DC Universe",
                    active: false, 
                },
                {
                    url: "#",
                    text: "DC Power Visa",
                    active: false, 
                },
            ],
            fourthList: [
                {
                    url: "#",
                    text: "Shop DC",
                    active: false, 
                },
                {
                    url: "#",
                    text: "Shop DC Collectibles",
                    active: false, 
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.footer {
    background-image: url(../assets/img/footer-bg.jpg);
    color: white;

    &__container-top {
        display: flex;
        justify-content: space-between;
    }

    &__logo {
        width: 40%;
    }

    &__container-bottom {
        width: 100%;
        height: 80px;
        background-color: $brand-footer-color;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

}

.footer__menu {
    width: 40%;
    display: flex;
    flex-wrap: wrap;
    padding-top: 1.5rem;
}

.footer__list {
    padding: 1rem;

    h3 {
        margin-bottom: .5rem;
        text-transform: uppercase;
        font-weight: 400;
        font-size: .9rem;
    }

    a {
        font-size: .6rem;
        color: gray;
        font-weight: 300;
    }
}

.footer__button {
        
        a {
            color: white;
            text-transform: uppercase;
            font-weight: 400;
            font-size: .8rem;
            border: 2px solid $brand-primary-color;
            padding: .7rem;
        }
}

.footer__social {

    span {
        text-transform: uppercase;
        color: $brand-primary-color;
        margin-right: .5rem;
    }

    img {
        width: 25px;
        margin: 0 .6rem;
    }
}

</style>