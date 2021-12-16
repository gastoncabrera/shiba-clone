<template>
  <div class="footer">
    <div class="footer__container custom_container custom_container--xxl">
      <nav class="footer_link">
        <ul class="footer_link__list">
          <li class="footer_link__item">
            <nuxt-link to="" class="footer_link__link">Medium</nuxt-link>
          </li>
          <li class="footer_link__item">
            <nuxt-link to="" class="footer_link__link">Etherscan</nuxt-link>
          </li>
          <li class="footer_link__item">
            <nuxt-link to="" class="footer_link__link">CoinMarketCap</nuxt-link>
          </li>
          <li class="footer_link__item">
            <nuxt-link to="" class="footer_link__link">CoinGecko</nuxt-link>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.footer {
  background-color: #18171f;
}

.footer__container {
  margin-top: 42px;
  margin-bottom: 22px;

  @include breakpoint(lg) {
    margin-bottom: 38px;
  }
}

.footer_link {
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer_link__list {
  display: flex;
  flex-wrap: wrap;
  list-style: none;
  justify-content: center;
}

.footer_link__item {
  margin-bottom: 16px;
  margin-left: 16px;
  margin-right: 16px;

  @include breakpoint(lg) {
    margin-bottom: 0;
  }
}

.footer_link__link {
  font-family: $font_1;
  color: #fff;
  font-size: 16px;
  line-height: 26px;
  text-decoration: none;
  transition: box-shadow 200ms ease;
}

.footer_link__link:hover {
  transition: box-shadow 200ms ease;
  box-shadow: inset 0 -1px 0 0 hsl(0deg 0% 100% / 30%);
}
</style>