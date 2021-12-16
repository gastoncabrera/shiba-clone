<template>
  <div class="art">
    <div class="art__container custom_container custom_container--xxl">
      <div class="art__wrap">
        <h2 class="art__title">Art</h2>
        <p class="art__description">
          We are proud to support ingenuity in all its forms with the
          <strong class="text_orange">Shiba Inu Incubator</strong>. The ShibArmy
          is made up of talented individuals who have united to build something
          remarkable, and we support this by cultivating an environment which
          encourages creativity and growth. Through the power of the Shiba Inu
          Incubator, we help holders find the tools they need to bring their
          inspiration and unique perspectives to life. This as just another way
          to encourage others to step outside of preconceived limits and
          regulations and experience what it means to be part of our
          decentralized movement.
        </p>
      </div>
    </div>
    <div class="carousel"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.art {
  background-color: #1c1b24;
}

.art__container {
  display: flex;
  flex-direction: column;
  padding-top: 60px;
  padding-bottom: 60px;

  @include breakpoint(sm) {
    padding-top: 80px;
    padding-bottom: 80px;
  }

  @include breakpoint(xl) {
    padding-top: 120px;
    padding-bottom: 150px;
  }
}

.art__wrap {
  max-width: 1194px;
  margin: 0 auto;
}

.art__title {
  font-family: $font_1;
  font-size: 30px;
  line-height: 42px;
  color: white;
  text-align: center;
  margin-bottom: 24px;

  @include breakpoint(sm) {
    font-size: 36px;
    line-height: 52px;
  }

  @include breakpoint(lg) {
    font-size: 48px;
    line-height: 66px;
  }
}

.art__description {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  color: #bbbbbe;
  text-align: center;

  @include breakpoint(sm) {
    font-size: 18px;
    line-height: 32px;
  }
}

.text_orange {
  color: #f28b03;
}

.carousel {
  width: 100%;
  height: 300px;
  border: 1px solid red;
}
</style>