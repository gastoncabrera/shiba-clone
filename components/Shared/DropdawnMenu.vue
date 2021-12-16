<template>
  <div :class="open ? 'dropdawn' : 'dropdawn dropdawn--open'">
    <div class="dropdawn__container custom_container custom_container--xxl">
      <Logo />

      <nav class="dropdawn_menu">
        <ul class="dropdawn_menu__list">
          <li class="dropdawn_menu__item">
            <nuxt-link to="" class="dropdawn_menu__link">Ecosystem</nuxt-link>
          </li>

          <li class="dropdawn_menu__item">
            <nuxt-link to="" class="dropdawn_menu__link">Buy</nuxt-link>
          </li>

          <li class="dropdawn_menu__item">
            <nuxt-link to="" class="dropdawn_menu__link">ShibaSwap</nuxt-link>
          </li>

          <li class="dropdawn_menu__item">
            <nuxt-link to="" class="dropdawn_menu__link">Art</nuxt-link>
          </li>

          <li class="dropdawn_menu__item">
            <nuxt-link to="" class="dropdawn_menu__link">Rescue</nuxt-link>
          </li>

          <li class="dropdawn_menu__item">
            <nuxt-link to="" class="dropdawn_menu__link">Community</nuxt-link>
          </li>

          <li class="dropdawn_menu__item">
            <div class="dropdawn_menu__link dropdawn_menu__link--en">
              EN
              <img src="lang-arr.svg" alt="" class="dropdawn_menu__img" />
            </div>
          </li>

          <li class="dropdawn_menu__item">
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
    </div>
  </div>
</template>

<script>
import Logo from "@/components/Shared/Logo.vue";

export default {
  components: { Logo },

  props: {
    open: {
      typeof: Boolean,
      require: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.dropdawn {
  position: fixed;
  top: -100vh;
  left: 0;
  height: 100vh;
  width: 100vw;
  z-index: 25;
  background-color: #1e1e29;
  transition: 500ms linear;

  @include breakpoint(xl) {
    display: none;
  }
}

.dropdawn--open {
  top: 0;
  transition: 500ms linear;
}

.dropdawn__container {
  margin-top: 20px;
}

.dropdawn_menu__list {
  list-style: none;
}

.dropdawn_menu__item {
  margin-top: 40px;
  margin-right: 40px;
}

.dropdawn_menu__link {
  font-family: $font_1;
  font-size: 30px;
  line-height: 42px;
  font-weight: 700;
  color: white;
  text-decoration: none;

  &:hover {
    color: #f28b03;
  }
}

.dropdawn_menu__link--en {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 20px;
  padding-bottom: 20px;
  border-top: 1px solid hsla(0, 0%, 100%, 0.1);
  border-bottom: 1px solid hsla(0, 0%, 100%, 0.1);
}

.dropdawn_menu__img {
  width: 16px;
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
  text-decoration: none;
  font-family: $font_1;
  font-size: 16px;
  color: #fff;
  line-height: 26px;
  font-weight: 700;
}
</style>