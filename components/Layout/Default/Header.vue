<template>
  <div class="header">
    <div class="header__container custom_container custom_container--xxl">
      <Logo />

      <MenuIcon @Dropdawn="dropdawn()" />

      <nav class="header_menu">
        <ul class="header_menu__list">
          <li class="header_menu__item">
            <nuxt-link to="" class="header_menu__link">Ecosystem</nuxt-link>
          </li>

          <li class="header_menu__item">
            <nuxt-link to="" class="header_menu__link">Buy</nuxt-link>
          </li>

          <li class="header_menu__item">
            <nuxt-link
              to=""
              class="header_menu__link header_menu__link--shibaswap"
            >
              ShibaSwap
            </nuxt-link>
          </li>

          <li class="header_menu__item">
            <nuxt-link to="" class="header_menu__link header_menu__link--more">
              More
              <img src="lang-arr.svg" alt="" class="header_menu__ico" />
            </nuxt-link>
          </li>

          <li class="header_menu__item">
            <nuxt-link
              to=""
              class="header_menu__link header_menu__link--more_active"
            >
              Art
            </nuxt-link>
          </li>

          <li class="header_menu__item">
            <nuxt-link
              to=""
              class="header_menu__link header_menu__link--more_active"
            >
              Rescue
            </nuxt-link>
          </li>

          <li class="header_menu__item">
            <nuxt-link
              to=""
              class="header_menu__link header_menu__link--more_active"
            >
              Community
            </nuxt-link>
          </li>

          <li class="header_menu__item">
            <div class="header_menu__link header_menu__link--line"></div>
          </li>

          <li class="header_menu__item">
            <nuxt-link
              to=""
              class="header_menu__link header_menu__link--languaje"
            >
              EN
              <img src="lang-arr.svg" alt="" class="header_menu__ico" />
            </nuxt-link>
          </li>

          <li class="header_menu__item">
            <nuxt-link to="" class="header_menu__link">
              <v-btn class="shiba_swap__button">
                <img
                  src="swap-ico.svg"
                  alt=""
                  class="shiba_swap__button_image"
                />

                <span class="shiba_swap__button_text">Use ShibaSwap</span>
              </v-btn>
            </nuxt-link>
          </li>
        </ul>
      </nav>

      <DropdawnMenu :open="open" />
    </div>
  </div>
</template>

<script>
import MenuIcon from "@/components/Home/MenuIcon.vue";
import DropdawnMenu from "@/components/Shared/DropdawnMenu.vue";
import Logo from "@/components/Shared/Logo.vue";

export default {
  components: { MenuIcon, DropdawnMenu, Logo },

  data() {
    return {
      open: true,
    };
  },

  methods: {
    dropdawn() {
      this.open = !this.open;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.header {
  background-color: #1f1e29;
}

.header__container {
  margin-top: 16px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;

  @include breakpoint(xl) {
    margin-top: 24px;
  }
}

.header_menu {
  display: none;

  @include breakpoint(xl) {
    display: block;
  }
}

.header_menu__list {
  list-style: none;
  display: flex;
  align-items: center;
}

.header_menu__link {
  font-family: $font_1;
  font-size: 16px;
  line-height: 26px;
  color: white;
  text-decoration: none;
  margin-right: 11px;
  margin-left: 11px;
  padding: 7px 5px;

  &:hover {
    color: #f28b03;
  }
}

.header_menu__ico {
  margin-left: 5px;
}

.header_menu__link--languaje {
  padding: 16px 20px;
}

.header_menu__link--more {
  @include breakpoint(xxl) {
    display: none;
  }
}

.header_menu__link--line {
  width: 1px;
  height: 30px;
  padding: 0;
  margin: 0;
  background-color: hsla(0, 0%, 100%, 0.1);
}

.header_menu__link--more_active,
.header_menu__link--shibaswap {
  display: none;

  @include breakpoint(xxl) {
    display: block;
  }
}

.shiba_swap__button_image {
  margin-right: 16px;
}

.shiba_swap__button.shiba_swap__button.shiba_swap__button {
  background-color: #1f1e29;
  border-radius: 200px;
  border: 1px solid #f17d02;
  padding: 24px 20px;
  font-family: $font_1;
  font-size: 16px;
  color: #fff;
  line-height: 26px;
  font-weight: 700;
  text-transform: capitalize;

  @include breakpoint(sm) {
    padding: 28px 20px;
    font-size: 18px;
  }
}

.shiba_swap__button_text.shiba_swap__button_text.shiba_swap__button_text {
  font-family: $font_1;
  font-size: 16px;
  color: #fff;
  line-height: 26px;
  font-weight: 700;
}
</style>