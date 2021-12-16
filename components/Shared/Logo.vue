<template>
  <nuxt-link to="" class="logo">
    <img src="shib-logo.svg" alt="" class="logo__image" />
    <div class="logo__text_wrap">
      <div class="logo__text logo__text--primary">SHIBA TOKEN</div>
      <div class="logo__text logo__text--hover">SHIBA TOKEN</div>
    </div>
  </nuxt-link>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.logo {
  text-decoration: none;
  display: flex;
  height: 40px;
  overflow: hidden;

  @include breakpoint(sm) {
    height: 48px;
  }

  @include breakpoint(xl) {
    height: 54px;
  }
}

.logo:hover .logo__text_wrap {
  transition: 150ms linear;
  margin-top: -45px;
}

.logo__image {
  margin-right: 18px;
}

.logo__text_wrap {
  transition: 150ms linear;
}

.logo__text {
  font-family: $font_1;
  font-size: 18px;
  line-height: 32px;
  font-weight: 800;
  margin-top: 8px;
  color: white;

  @include breakpoint(sm) {
    margin-top: 10px;
    font-size: 22px;
  }

  @include breakpoint(lg) {
    margin-top: 12px;
    font-size: 24px;
  }
}

.logo__text--hover {
  color: #f28b03;
}
</style>