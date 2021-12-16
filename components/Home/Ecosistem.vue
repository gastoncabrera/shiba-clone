<template>
  <div class="ecosystem">
    <div class="ecosystem__container custom_container custom_container--xxl">
      <div class="ecosystem__content">
        <h2 class="ecosystem__title">Our Project & Ecosystem</h2>

        <p class="ecosystem__description">
          From its inception, Shiba Inu has done things differently. Starting
          with a supply of 1 quadrillion, our founder, Ryoshi, locked 50% in
          Uniswap, then “burned” the other half to Ethereum co-founder
          <span
            class="ecosystem__description ecosystem__description--text_white"
          >
            Vitalik Buterin
          </span>
          for safekeeping.
          <br />
          <br />
          To help reverse the devastating spread of Covid-19 in India, VB has
          since utilized SHIB in the largest crypto donation in history, and
          then
          <span
            class="ecosystem__description ecosystem__description--text_white"
          >
            actually
          </span>
          burned 40% of its total supply to a dead wallet, ensuring our
          long-term success and stability. In the words of Ryoshi, “Thank you to
          the woofmeister for enabling true decentralization. Now we truly
          begin.”
        </p>
      </div>
      <div class="ecosystem__buttons">
        <CardLink
          text="Liquidity Locked to Uniswap"
          imgBg="/ico-uni-col.svg"
          img="/ico-uni.svg"
        />

        <CardLink
          text="India's Covid Relief Fund"
          imgBg="/ico-icr-b.png"
          img="/ico-icr.png"
        />

        <CardLink
          text="Vitalik Buterin Burn"
          imgBg="/ico-vb-burn-f.svg"
          img="/ico-vb-burn.svg"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardLink from "@/components/Home/CardLink";

export default {
  components: {
    CardLink,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.ecosystem {
  position: relative;
  z-index: 2;
  background-color: #1c1b24;
  padding-top: 60px;
  padding-bottom: 51px;

  @include breakpoint(sm) {
    padding-top: 80px;
    padding-bottom: 64px;
  }

  @include breakpoint(lg) {
    padding-bottom: 80px;
  }

  @include breakpoint(xl) {
    padding-top: 120px;
    padding-bottom: 152px;
  }
}

.ecosystem__container {
  @include breakpoint(lg) {
    display: flex;
    justify-content: space-between;
  }
}

.ecosystem__content {
  max-width: 619px;
  @include breakpoint(lg) {
    margin-right: 60px;
  }
}

.ecosystem__title {
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

.ecosystem__description {
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

.ecosystem__description--text_white {
  color: #fff;
  font-weight: 700;
}

.ecosystem__buttons {
  @include breakpoint(sm) {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
  }
}
</style>