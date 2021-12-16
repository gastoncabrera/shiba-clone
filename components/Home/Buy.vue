<template>
  <div class="buy">
    <div class="buy__container custom_container custom_container--xxl">
      <div class="buy__left">
        <h2 class="buy__title">How to Buy</h2>

        <p class="buy__description">
          SHIB and LEASH are best purchased and sold through
          <strong class="text-white">ShibaSwap</strong>, but can also be found
          on Uniswap and an ever-growing list of CEXs. Please note that, outside
          of ShibaSwap, exchanges which support one may not support the other.
          <br />
          <br />
          SHIB is a decentralized experiment and, as such, we always incentivize
          the use of DEXs. If you choose to utilize a CEX instead, remember to
          research it first to ensure it is both safe and secure.
        </p>

        <div class="buy__buttons">
          <Btn title="Buy SHIB" class="btn" />

          <Btn title="Buy LEASH" class="btn" />

          <Btn title="Buy BONE" class="btn" />
        </div>
      </div>

      <div class="buy__right">
        <img src="c1.png" alt="" class="buy__image" />

        <div class="buy__blur_container">
          <img src="bc1.png" alt="" class="buy__blur_one" />

          <img src="bc2.png" alt="" class="buy__blur_two" />

          <img src="bc4.png" alt="" class="buy__blur_three" />
        </div>

        <div class="buy__coin_container">
          <img src="bone_coin-2.png" alt="" class="buy__coin_one" />

          <img src="leash_coin-1.png" alt="" class="buy__coin_two" />

          <img src="shiba_coin-1.png" alt="" class="buy__coin_three" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Btn from "@/components/Shared/Btn";

export default {
  components: {
    Btn,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.buy {
  background-color: #1c1b24;
}

.buy__container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 104px;
  padding-bottom: 60px;

  @include breakpoint(lg) {
    flex-direction: row;
    justify-content: space-between;
  }
}

.buy__left {
  order: 2;
  text-align: center;
  width: 100%;
  max-width: 619px;

  @include breakpoint(lg) {
    order: 1;
    margin-right: 100px;
  }
}

.buy__title {
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

.buy__description {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  color: #bbbbbe;
  text-align: center;
  margin-bottom: 40px;

  @include breakpoint(sm) {
    text-align: left;
    font-size: 18px;
  }
}

.text-white {
  color: white;
}

.buy__buttons {
  display: flex;
  margin-top: 48px;
  flex-wrap: wrap;

  @include breakpoint(sm) {
    flex-wrap: nowrap;
  }
}

.btn {
  margin-right: 8px;
  margin-left: 8px;
  margin-bottom: 16px;
}

.buy__right {
  min-width: 350px;
  max-width: 450px;
  min-height: 350px;
  max-width: 450px;
  order: 1;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 91px;

  @include breakpoint(lg) {
    order: 2;
  }
}

.buy__image {
  width: 190px;
}

.buy__blur_container {
  width: 100%;
  min-width: 350px;
  max-width: 450px;
  min-height: 350px;
  max-width: 450px;
  position: absolute;
  top: 0;
}

.buy__blur_one {
  position: absolute;
  top: -80px;
  left: 50%;
  transform: translateX(-50%);
  width: 144px;
  z-index: 10;
}

.buy__blur_two {
  position: absolute;
  bottom: -30px;
  left: -30px;
  width: 134px;
  z-index: 10;
}

.buy__blur_three {
  position: absolute;
  bottom: -20px;
  right: -20px;
  width: 117px;
  z-index: 10;
}

.buy__coin_container {
  position: absolute;
  top: 0;
  width: 100%;
  min-width: 350px;
  max-width: 450px;
  min-height: 350px;
  max-width: 450px;
  border: 1px dashed rgb(148, 148, 148);
  border-radius: 200%;
}

.buy__coin_one {
  position: absolute;
  top: 20px;
  left: 0;
  width: 72px;
}

.buy__coin_two {
  position: absolute;
  top: 20px;
  right: 0;
  width: 72px;
}

.buy__coin_three {
  position: absolute;
  bottom: -40px;
  left: 50%;
  transform: translateX(-50%);
  width: 72px;
}
</style>

