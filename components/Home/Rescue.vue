<template>
  <div class="rescue">
    <div class="rescue__container custom_container custom_container--xxl">
      <div class="rescue__left">
        <h2 class="rescue__title">Rescue</h2>
        <p class="rescue__description">
          From the tips of their noses to the ends of their tails, Shiba Inu are
          intelligent, brave, and independent, with an equal propensity for
          loyalty and mischief. Sadly, the characteristics which make them
          extraordinary are the same ones which make them a challenging pet.
          Inexperienced owners can find themselves unprepared for a dog that’s
          known for its bold (i.e. stubborn) personality.
          <br />
          <br />
          Luckily, we are helping these dogs in real life! We use
          <strong class="text_orange">Amazon Smile</strong>
          to collect and donate a percentage of your Amazon purchases to the
          <strong class="text_white">Shiba Inu Rescue Association</strong>.
          Joining is easy and free! Just use
          <nuxt-link to="" class="text_orange"
            ><strong>smile.amazon.com</strong></nuxt-link
          >
          when placing orders and select Shiba Inu Rescue Association (a
          501(c)3, preferred non-profit organization). You’re seconds away from
          helping Shibs in need. Start funding shelters today.
        </p>
      </div>
      <div class="rescue__right">
        <v-btn class="rescue__button">Rescue Me</v-btn>
        <div class="rescue__image_container">
          <img src="meat-2.svg" alt="" class="rescue__image_one" />
          <img src="meat-3.svg" alt="" class="rescue__image_two" />
          <img src="meat-1.svg" alt="" class="rescue__image_three" />
        </div>

        <img src="logo-amazon.svg" alt="" class="rescue__image_amazon" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.rescue {
  background-color: #1f1e29;
}

.rescue__container {
  padding-top: 60px;
  padding-bottom: 120px;

  @include breakpoint(sm) {
    padding-top: 80px;
    padding-bottom: 152px;
  }

  @include breakpoint(lg) {
    padding-bottom: 80px;
    display: flex;
  }

  @include breakpoint(xl) {
    padding-top: 120px;
    padding-bottom: 152px;
  }
}

.rescue__left {
  width: 100%;

  @include breakpoint(lg) {
    margin-right: 60px;
  }
}

.rescue__title {
  @include title;
}

.rescue__description {
  @include description;
}

.text_orange {
  color: #f28b03;
}

.text_white {
  color: white;
}

.rescue__right {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 100px;

  @include breakpoint(lg) {
    margin-top: 0;
  }
}

.rescue__image_container {
  position: absolute;
}

.rescue__image_one {
  position: absolute;
  top: -10px;
  right: 60px;
  width: 90px;

  @include breakpoint(sm) {
    width: 103px;
    right: 80px;
  }

  @include breakpoint(xl) {
    right: 110px;
  }
}

.rescue__image_two {
  position: absolute;
  top: 20px;
  left: 50px;
  width: 100px;

  @include breakpoint(sm) {
    width: 120px;
    top: 30px;
    left: 80px;
  }

  @include breakpoint(xl) {
    top: 40px;
    left: 150px;
  }
}

.rescue__image_three {
  position: absolute;
  bottom: 20px;
  left: 20px;
  width: 120px;

  @include breakpoint(sm) {
    width: 140px;
  }

  @include breakpoint(lg) {
    width: 160px;
  }

  @include breakpoint(xl) {
    left: 100px;
  }
}

.rescue__image_amazon {
  margin-top: 20px;
}
</style>
<style lang="scss">
@import "@/assets/scss/utils";

.rescue {
  .rescue__button.rescue__button.rescue__button {
    position: relative;
    font-family: $font_1;
    line-height: 26px;
    font-weight: 700;
    font-size: 20px;
    background-image: linear-gradient(84deg, #f28b03, #f06500);
    padding: 29px 48px 24px;
    text-transform: capitalize;
    margin: 0;
    height: 100%;
    letter-spacing: 1px;
    color: white;
    border-radius: 16px;

    @include breakpoint(sm) {
      padding: 36px 60px 28px;
      font-size: 24px;
      line-height: 40px;
    }

    @include breakpoint(lg) {
      height: 100px;
    }

    @include breakpoint(xl) {
      height: 110px;
      font-size: 36px;
      line-height: 52px;
    }
  }
}
</style>

