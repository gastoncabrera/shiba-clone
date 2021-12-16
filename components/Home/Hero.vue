<template>
  <div class="hero">
    <div class="hero__container custom_container custom_container--xxl">
      <h1 class="hero__title">
        A Decentralized Meme Token that Evolved into a Vibrant Ecosystem
      </h1>

      <p class="hero__subtitle">
        SHIB, LEASH, BONE — ShibaSwap — Innovative Reward System — The Shiba
        Incubator — And more. 585k+ Community Members and Growing Fast!
      </p>

      <div class="hero_buttons__container">
        <nuxt-link to="" class="hero_buttons__buy">How to Buy</nuxt-link>

        <nuxt-link to="" class="hero_buttons__woofpaper">
          Read WoofPaper v2
        </nuxt-link>
      </div>
      <div class="hero__wrap">
        <img src="/moon.svg" alt="" class="hero__wrap_moon" />

        <img src="/hero-shib.png" alt="" class="hero__wrap_shib" />
      </div>

      <nuxt-link to="" class="hero_scroll">
        <div class="hero_scroll__wrap">
          <img src="/hero-scroll-shape.svg" alt="" class="hero_scroll__image" />

          <img src="/hero-scroll-arr.svg" alt="" class="hero_scroll__arrow" />
        </div>
      </nuxt-link>
    </div>
    <img src="/bg-glow.svg" alt="" class="hero__shadow" />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.hero {
  position: relative;
  background-color: #1f1e29;
}

.hero__container {
  padding-top: 140px;
  color: white;
  position: relative;
  padding-bottom: 120px;
  position: relative;
  z-index: 10;

  @include breakpoint(sm) {
    padding-top: 190px;
    padding-bottom: 190px;
  }

  @include breakpoint(md) {
    padding-top: 240px;
    padding-bottom: 260px;
  }

  @include breakpoint(xl) {
    padding-top: 300px;
    padding-bottom: 300px;
  }

  @include breakpoint(xxxl) {
    height: 100vh;
  }
}

.hero__title {
  font-family: $font_1;
  font-size: 30px;
  line-height: 42px;
  text-align: center;
  margin-bottom: 24px;

  @include breakpoint(sm) {
    font-size: 36px;
    line-height: 52px;
    text-align: left;
  }

  @include breakpoint(lg) {
    font-size: 48px;
    line-height: 66px;
    max-width: 785px;
  }
}

.hero__subtitle {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  text-align: center;
  color: #bbbbbe;
  max-width: 550px;

  @include breakpoint(sm) {
    text-align: left;
    font-size: 18px;
    line-height: 32px;
    margin-right: 110px;
  }
}

.hero_buttons__container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-family: $font_1;
  font-size: 16px;
  font-weight: 700;
  line-height: 28px;

  @include breakpoint(sm) {
    align-items: flex-start;
  }

  @include breakpoint(md) {
    flex-direction: row;
    justify-content: flex-start;
  }
}

.hero_buttons__buy {
  text-decoration: none;
  background-image: linear-gradient(84deg, #f28b03, #f06500);
  padding: 13px 30px;
  border-radius: 50px;
  color: white;
}

.hero_buttons__buy:hover {
  background-image: linear-gradient(84deg, #f00500, #f00500);
}

.hero_buttons__woofpaper {
  text-decoration: none;
  color: white;
  padding: 13px 30px;
  border-radius: 50px;
  margin-top: 16px;
  border: 1px solid #f28b03;

  @include breakpoint(md) {
    margin-top: 0;
    margin-left: 16px;
  }
}

.hero__wrap {
  display: none;

  @include breakpoint(sm) {
    display: block;
    width: 100%;
    max-width: 260px;
  }
}

.hero__wrap_moon {
  max-width: 260px;
  position: absolute;
  bottom: 210px;
  right: -75px;

  @include breakpoint(md) {
    max-width: 450px;
    right: -175px;
    bottom: 120px;
  }

  @include breakpoint(xl) {
    max-width: 518px;
    bottom: 200px;
  }

  @include breakpoint(xxl) {
    max-width: 650px;
    bottom: 250px;
  }
}

.hero__wrap_shib {
  max-width: 260px;
  position: absolute;
  bottom: 0;
  right: -55px;

  @include breakpoint(md) {
    max-width: 280px;
    right: 0;
    margin-right: 50px;
  }

  @include breakpoint(xl) {
    max-width: 350px;
  }

  @include breakpoint(xxl) {
    max-width: 480px;
  }
}

.hero__shadow {
  position: absolute;
  left: -1284px;
  top: auto;
  right: auto;
  bottom: -1062px;
  z-index: 0;
  width: 2000px;
}

.hero_scroll {
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 10;

  @include breakpoint(sm) {
    left: 20px;
    bottom: -10px;
    transform: none;
    margin-left: 50px;
  }
}

.hero_scroll__wrap {
  position: relative;
  width: 100%;
  z-index: 10;
}

.hero_scroll__wrap:hover .hero_scroll__arrow {
  transition: 200ms linear;
  top: 60%;
}

.hero_scroll__arrow {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  transition: 200ms linear;
}
</style>