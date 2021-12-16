<template>
  <div class="social_link">
    <div class="social_link__container custom_container custom_container--xxl">
      <p class="social_link__text">
        Our community grows stronger every day. Please follow our social
        platforms to get the most up-to-date, accurate SHIB information.
        <br />
        <br />
        Using the links below, you can join our various groups alongside the
        <strong class="text_white">1M+</strong> other members of the ShibArmy.
      </p>
      <div class="social_link__country">
        Click here to search for your preferred country!
      </div>
      <nav class="social">
        <ul class="socia__list">
          <li class="social__item">
            <nuxt-link to="" class="social__link">
              <img src="ico-tel.svg" alt="" class="social__link_image" />
              <span class="social__link_text">Shiba Ecosystem Telegram</span>
            </nuxt-link>
          </li>
          <li class="social__item">
            <nuxt-link to="" class="social__link">
              <img src="ico-tw.svg" alt="" class="social__link_image" />
              <span class="social__link_text">Twitter</span>
            </nuxt-link>
          </li>
          <li class="social__item">
            <nuxt-link to="" class="social__link">
              <img src="ico-red.svg" alt="" class="social__link_image" />
              <span class="social__link_text">Reddit</span>
            </nuxt-link>
          </li>
          <li class="social__item">
            <nuxt-link to="" class="social__link">
              <img src="ico-dis.svg" alt="" class="social__link_image" />
              <span class="social__link_text">Discord</span>
            </nuxt-link>
          </li>
          <li class="social__item">
            <nuxt-link to="" class="social__link">
              <img src="instagram.svg" alt="" class="social__link_image" />
              <span class="social__link_text">Instagram</span>
            </nuxt-link>
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

.social_link {
  background-color: #1a1921;
  padding-top: 40px;
  padding-bottom: 40px;

  @include breakpoint(sm) {
    padding-top: 50px;
    padding-bottom: 50px;
  }

  @include breakpoint(lg) {
    padding-top: 80px;
    padding-bottom: 80px;
  }
}

.social_link__container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.social_link__text {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  color: #bbbbbe;
  text-align: center;
  width: 100%;
  max-width: 885px;

  @include breakpoint(sm) {
    font-size: 18px;
    line-height: 32px;
  }
}
.text_white {
  color: white;
}

.social_link__country {
  font-family: $font_1;
  font-size: 16px;
  line-height: 28px;
  font-weight: 700;
  text-align: center;
  color: white;
  margin-top: 32px;
  box-shadow: 0 1px 0 0 #fff;
  cursor: pointer;

  @include breakpoint(sm) {
    font-size: 18px;
    line-height: 32px;
  }

  &:hover {
    box-shadow: 0 1px 0 0 #f28b03;
    color: #f28b03;
  }
}

.social {
  margin-top: 40px;
  width: 100%;
  max-width: 500px;

  @include breakpoint(sm) {
    margin-top: 50px;
  }

  @include breakpoint(lg) {
    margin-top: 80px;
    max-width: none;
  }
}

.socia__list {
  display: flex;
  justify-content: center;
  align-items: center;
  list-style: none;
  flex-wrap: wrap;
}

.social__link {
  display: flex;
  flex-direction: column;
  align-items: center;
  min-width: 74px;
  margin: 20px;
  text-decoration: none;
  font-family: $font_1;
  font-size: 12px;
  line-height: 19px;
  color: rgb(187, 187, 190);
  transition: 300ms linear;

  @include breakpoint(sm) {
    margin: 25px;
  }

  @include breakpoint(lg) {
    margin-left: 30px;
    margin-right: 30px;
  }

  @include breakpoint(xl) {
    margin: 0;
    margin-left: 35px;
    margin-right: 35px;
  }
}

.social__link:hover {
  color: white;
}

.social__link:hover .social__link_image {
  transition: 300ms linear;
  transform: scale(1.1);
}

.social__link_image {
  height: 56px;
  margin-bottom: 18px;
}

.social__link_text {
  text-align: center;
}
</style>