<template>
  <div class="coins">
    <div class="coins__container custom_container custom_container--xxl">
      <BoxCoin :title="'Buy SHIB'" :img="'shiba_coin-1.png'">
        <template v-slot:description>
          <p class="box_coin__description">
            The Shiba Inu token is our foundational currency that allows
            investors to hold millions, billions, or even trillions, of it in
            their wallets.
            <br />
            <br />
            Between its international recognition and its legitimate utility,
            <strong class="text_orange">SHIB</strong> is up thousands of times
            and is constantly expanding its reach. SHIB is the first to be
            listed and incentivized on ShibaSwap, our proprietary DEX.
          </p>
        </template>
      </BoxCoin>

      <BoxCoin :title="'Buy LEASH'" :img="'leash_coin-1.png'">
        <template v-slot:description>
          <p class="box_coin__description">
            <strong class="text_orange">LEASH</strong> was originally set to be
            a rebase token, but then we removed the rebase and unleashed its
            full potential. With a total supply of ONLY
            <strong class="text_white">107,646 tokens</strong>, it represents
            the other end of our Ecosystem spectrum.
            <br />
            <br />
            LEASH is the second token incentivized on ShibaSwap and will offer
            lucrative rewards for the holders providing its liquidity.
          </p>
        </template>
      </BoxCoin>

      <BoxCoin :title="'Buy BONE'" :img="'bone_coin-2.png'">
        <template v-slot:description>
          <p class="box_coin__description">
            <strong class="text_orange">BONE</strong> has 250,000,000 tokens,
            and is designed to fit perfectly between the previous two tokens in
            regards to circulation supply.
            <br />
            <br />
            Moreover, the token is a Governance token which will allow the
            #ShibArmy to vote on upcoming proposals on our
            <strong class="text_orange">Doggy DAO</strong>.
          </p>
        </template>
      </BoxCoin>
    </div>
  </div>
</template>

<script>
import BoxCoin from "@/components/Home/BoxCoin";

export default {
  components: {
    BoxCoin,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.coins {
  background-color: #1f1e29;
  padding: 100px 0;
}

.coins__container {
  display: grid;
  align-items: flex-start;
  grid-column-gap: 32px;
  grid-row-gap: 32px;

  @include breakpoint(lg) {
    grid-template-columns: repeat(2, 1fr);
  }

  @include breakpoint(xl) {
    grid-template-columns: repeat(3, 428px);
    grid-column-gap: 40px;
    grid-row-gap: 40px;
  }
}

.box_coin__description {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  color: #bbbbbe;
  text-align: center;

  @include breakpoint(sm) {
    text-align: left;
    font-size: 18px;
  }
}

.text_orange {
  color: #f28b03;
}

.text_white {
  color: white;
}
</style>