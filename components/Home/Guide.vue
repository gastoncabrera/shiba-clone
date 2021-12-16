<template>
  <div class="guide">
    <div class="guide__container custom_container custom_container--xxl">
      <h2 class="guide__title">Quick Start Guide</h2>

      <div class="guide__box">
        <GuideBox
          :id="1"
          :title="'Create MetaMask wallet'"
          :description="'Create a MetaMask Wallet using either a desktop computer or an iOS/Android mobile device. That will allow you to buy, sell, send, and receive SHIB or LEASH.'"
        />

        <GuideBox
          :id="2"
          :title="'Send ETH to your wallet'"
          :description="'You can buy Ethereum (ETH) directly on MetaMask or transfer it to your MetaMask Wallet from exchanges like Coinbase, Binance, etc. Make sure to use the ERC-20 network when transfering ETH.'"
        />

        <GuideBox
          :id="3"
          :title="'Connect your wallet to ShibaSwap'"
          :description="'Access your wallet to ShibaSwap by clicking ‘Connect to a wallet’ and selecting MetaMask.'"
        />

        <GuideBox
          :show="false"
          :id="4"
          :title="'Swap ETH for SHIB, LEASH or BONE'"
          :description="'You can start swapping as soon as you have ETH available! Press ‘Select a token’ and enter the token address or search for it on the tokens list.'"
        />
      </div>
    </div>
  </div>
</template>

<script>
import GuideBox from "@/components/Home/GuideBox";

export default {
  components: {
    GuideBox,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.guide {
  background-color: #1c1b24;
}

.guide__container {
  padding-top: 50px;
  padding-bottom: 50px;

  @include breakpoint(xl) {
    padding-bottom: 152px;
  }
}

.guide__title {
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
    margin-bottom: 80px;
  }
}

.guide__box {
  background-color: #18171f;
  border-radius: 16px;
  padding-top: 32px;
  padding-left: 32px;
  padding-right: 32px;
  padding-bottom: 48px;

  @include breakpoint(sm) {
    padding-left: 40px;
    padding-right: 40px;
  }

  @include breakpoint(xl) {
    padding-left: 80px;
    padding-right: 80px;
    margin-top: 48px;
  }
}

.guide__wrap {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: white;

  @include breakpoint(sm) {
    align-items: flex-start;
  }

  @include breakpoint(lg) {
    flex-direction: row;
  }
}

.guide__left {
  display: flex;
  flex-direction: column;

  @include breakpoint(lg) {
    flex-direction: row;
    align-items: center;
  }
}

.guide__id {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background-color: #23212c;
  padding: 20px;
  margin-bottom: 20px;
  display: flex;
  justify-content: center;
  align-items: center;

  @include breakpoint(lg) {
    margin-bottom: 0;
    width: 70px;
    height: 70px;
  }

  @include breakpoint(lg) {
    width: 80px;
    height: 80px;
  }
}

.guide__id_number {
  font-family: $font_1;
  font-size: 20px;
  line-height: 42px;
  font-weight: 300;
  display: flex;
  height: 100%;
  align-items: center;

  @include breakpoint(lg) {
    font-size: 24px;
  }
}

.guide__title_wrap {
  font-family: $font_1;
  font-size: 24px;
  line-height: 35px;
  margin-bottom: 24px;

  @include breakpoint(sm) {
    font-size: 30px;
    line-height: 42px;
  }
}

.guide__line {
  display: none;

  @include breakpoint(lg) {
    display: flex;
    height: 1px;
    width: 50px;
    background-color: #f28b03;
    margin-right: 24px;
    margin-left: 24px;
  }
}

.guide__right {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;

  @include breakpoint(sm) {
    align-items: flex-start;
    text-align: left;
  }

  @include breakpoint(lg) {
    padding-top: 18px;
    padding-right: 35px;
  }
}

.guide__description_wrap {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  color: #bbbbbe;

  @include breakpoint(sm) {
    font-size: 18px;
    line-height: 32px;
  }
}

.guide__line_divider {
  width: 100%;
  height: 1px;
  background-color: #292831;
  margin-top: 40px;
  margin-bottom: 40px;
}
</style>