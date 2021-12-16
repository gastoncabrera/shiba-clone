<template>
  <div class="banner">
    <div class="banner__container custom_container custom_container--xxl">
      <div class="banner__text">
        Shytoshi, our Project Manager is in the process of verification. This is
        to let Twitter know that his official Twitter account is found at
        <nuxt-link to="" class="banner__text"
          >www.twitter.com/ShytoshiKusama.</nuxt-link
        >
        <br />
        Verification will help us stop scammers of our million person Community
        in our other verified account
        <nuxt-link to="" class="banner__text">@Shibtoken. </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.banner {
  display: none;
  background-color: #f06500;

  @include breakpoint(xl) {
    display: flex;
  }
}

.banner__container {
  padding: 10px;
  max-width: 2000px;
}

.banner__text {
  font-family: $font_2;
  font-size: 16px;
  color: white;
  text-align: center;
}
</style>