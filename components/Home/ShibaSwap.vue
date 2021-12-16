<template>
  <div class="shiba_swap">
    <div class="shiba_swap__container custom_container custom_container--xxl">
      <div class="shiba_swap__left">
        <div class="shiba_swap__wrap_image">
          <img src="swap-img.png" alt="" class="shiba_swap__image" />

          <img src="coin-shad-1.png" alt="" class="shiba_swap__shadow" />
        </div>
        <nuxt-link to="" class="shiba_swap__link">
          <v-btn class="shiba_swap__button">
            <img src="swap-ico.svg" alt="" class="shiba_swap__button_image" />

            <span class="shiba_swap__button_text">Use ShibaSwap</span>
          </v-btn>
        </nuxt-link>
      </div>

      <div class="shiba_swap__right">
        <h2 class="shiba_swap__title">ShibaSwap</h2>

        <div class="certik__wrap">
          <div class="certik__left">
            <img src="certik-logo.svg" alt="" class="certik__image" />

            <div class="certik__status">
              <div class="certik__status_icon"></div>

              <span class="certik__status_text">On board</span>
            </div>
          </div>

          <div class="certik__right">
            <v-btn class="certik__button">
              <img src="ico-eye.svg" alt="" class="certik__button_image" />

              <span class="certik__button_text"> Audit Report </span>
            </v-btn>
          </div>
        </div>

        <p class="shiba_swap__description">
          SHIB, LEASH, and BONE, come together to create
          <strong class="text_orange">ShibaSwap</strong>, the next evolution in
          DeFi platforms. ShibaSwap gives users the ability to
          <strong class="text_white">DIG</strong> (provide liquidity),
          <strong class="text_white">BURY</strong> (stake), and
          <strong class="text_white">SWAP</strong> tokens to gain
          <strong class="text_white">WOOF</strong
          ><strong class="text_white">Returns</strong> through our sophisticated
          and innovative passive income reward system.
          <br />
          <br />
          Our platform also allows the ShibArmy to access upcoming NFTs and
          additional tools, such as portfolio trackers, to make navigating the
          crypto world simple and intuitive.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.shiba_swap {
  background-color: #1f1e29;
}

.shiba_swap__container {
  display: flex;
  flex-direction: column;
  padding-top: 60px;
  padding-bottom: 60px;

  @include breakpoint(sm) {
    padding-top: 80px;
    padding-bottom: 80px;
  }

  @include breakpoint(lg) {
    flex-direction: row;
    align-items: center;
  }

  @include breakpoint(xl) {
    padding-top: 120px;
    padding-bottom: 150px;
  }
}

.shiba_swap__left {
  order: 2;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;

  @include breakpoint(lg) {
    order: 1;
    margin-right: 5%;
  }
}

.shiba_swap__wrap_image {
  position: relative;
}

.shiba_swap__image {
  width: 100%;
  max-width: 500px;
  position: relative;
  z-index: 10;

  @include breakpoint(xl) {
    max-width: 650px;
  }
}

.shiba_swap__shadow {
  position: absolute;
  bottom: -200px;
  left: 0;
  width: 100%;
}

.shiba_swap__link {
  text-decoration: none;
}

.shiba_swap__button_image {
  margin-right: 16px;
}

.shiba_swap__right {
  order: 1;
  width: 100%;

  @include breakpoint(lg) {
    order: 2;
    margin-left: 5%;
  }
}

.shiba_swap__title {
  font-family: $font_1;
  font-size: 30px;
  line-height: 42px;
  color: white;
  text-align: center;
  margin-bottom: 24px;

  @include breakpoint(sm) {
    text-align: left;
    font-size: 36px;
    line-height: 52px;
  }

  @include breakpoint(lg) {
    font-size: 48px;
    line-height: 66px;
  }
}

.certik__wrap {
  display: flex;
  flex-direction: column;
  align-items: center;
  border-radius: 16px;
  background-color: #18171f;
  margin-bottom: 40px;
  padding: 24px 30px;

  @include breakpoint(xxl) {
    flex-direction: row;
    justify-content: space-between;
  }
}

.certik__left {
  @include breakpoint(xl) {
    display: flex;
  }
}

.certik__image {
  height: 32px;
}

.certik__status {
  display: flex;
  align-items: center;
  justify-content: center;

  @include breakpoint(xl) {
    margin-left: 24px;
  }
}

.certik__status_icon {
  height: 8px;
  width: 8px;
  border-radius: 100%;
  background-color: #0f9713;
}

.certik__status_text {
  font-family: $font_1;
  font-size: 14px;
  line-height: 32px;
  margin-left: 8px;
  color: white;
}

.certik__button_image {
  margin-right: 8px;
}

.certik__button_text {
  font-family: $font_1;
  font-size: 16px;
  color: #fff;
  line-height: 26px;
  font-weight: 700;
}

.shiba_swap__description {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  color: #bbbbbe;
  text-align: center;

  @include breakpoint(sm) {
    font-size: 18px;
    text-align: left;
  }
}

.text_orange {
  color: #f28b03;
}

.text_white {
  color: white;
}
</style>

<style lang="scss">
@import "@/assets/scss/utils";

.shiba_swap {
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
    margin-top: 30px;

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

  .certik__button.certik__button.certik__button {
    border-radius: 200px;
    border: 1px solid #f17d02;
    background-color: transparent;
    padding: 24px 20px;
  }
}
</style>
