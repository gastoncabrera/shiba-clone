<template>
  <div class="community">
    <div class="community__container custom_container custom_container--xxl">
      <h1 class="community__title">Community</h1>
      <p class="community__description">
        If you'd like to donate to the <strong class="text_white">Devs</strong>,
        send <strong class="text_orange">ETH</strong>,
        <strong class="text_orange">SHIB</strong>,
        <strong class="text_orange">LEASH</strong> or
        <strong class="text_orange">BONE</strong> here. Thank you for your
        support! WOOF!
      </p>
      <div class="community__wrap">
        <div class="community__left">
          <div class="community__code">
            0xc351155C80aCD043BD5F8FE7ffc8536af1fF9375
          </div>
          <div class="community__shadow"></div>
        </div>
        <div class="community__right">
          <v-btn class="community__buttom">
            <img src="ico-copy.svg" alt="" class="community__buttom_image" />
            <span class="community__buttom_text">Copy to Clipboard</span>
          </v-btn>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.community {
  border-bottom: 1px solid #292831;
  background-color: #1c1b24;
}

.community__container {
  padding-top: 60px;
  padding-bottom: 60px;
  display: flex;
  flex-direction: column;
  align-items: center;

  @include breakpoint(sm) {
    padding-top: 80px;
    padding-bottom: 80px;
  }

  @include breakpoint(xl) {
    padding-top: 120px;
  }

  @include breakpoint(xl) {
  }
}

.community__title {
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

.community__description {
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

.text_white {
  color: white;
}

.text_orange {
  color: #f28b03;
}

.community__wrap {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 37px 30px;
  border-radius: 16px;
  background-color: #18171f;
  margin-top: 40px;

  @include breakpoint(lg) {
    flex-direction: row;
  }
}

.community__left {
  position: relative;
  overflow: hidden;
  width: 350px;
}

.community__code {
  font-family: $font_1;
  font-size: 18px;
  line-height: 32px;
  color: white;
  width: 100%;
  max-width: 250px;
}

.community__shadow {
  position: absolute;
  left: auto;
  top: 0%;
  right: 0%;
  bottom: 0%;
  width: 50%;
  background-image: linear-gradient(270deg, #18171f 22%, rgba(24, 23, 31, 0));
}

.community__right {
}

.community__buttom.community__buttom.community__buttom {
  border-radius: 200px;
  border: 1px solid #f17d02;
  background-color: transparent;
  padding: 24px 20px;
  text-transform: capitalize;
  margin-top: 20px;

  @include breakpoint(lg) {
    margin-top: 0;
  }
}

.community__buttom_image {
  margin-right: 8px;
}

.community__buttom_text {
  font-family: $font_1;
  font-size: 16px;
  color: #fff;
  line-height: 26px;
  font-weight: 700;
}
</style>