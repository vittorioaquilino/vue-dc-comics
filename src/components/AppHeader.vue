<template>
  <header class="header">
    <div class="header__container container">
      <div class="header__logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <nav>
        <div class="header__menu">
          <ul>
            <li
            v-for="(element, index) in links"
            :key="index"
            :class="element.active === true ? 'active' : ''"
            >
                <a href="">{{ element.text}}</a>
            </li>
          </ul>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
      return {
          links: [
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
      }
  }
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.header {
  height: 100px;
  padding: 0.5rem;

    &__logo {
        img {
            width: 70px;
        }
    }

    &__menu {
        ul {
            display: flex;

        }

        li {
            padding:2.35rem .8rem;
            text-transform: uppercase;
            font-size: .7rem;
            font-weight: 500;
            border-bottom: 3px solid trasparent;
            

            &.active {
                border-bottom: 4px solid $brand-primary-color;
            }

            &.active a {
                color: $brand-primary-color;
            }
        }

        a {
            color: black;
        }
    }

}

.header__container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>
