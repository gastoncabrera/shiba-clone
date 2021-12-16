<template>
  <div class="button">
    <nuxt-link to="" class="button__link">
      <v-btn class="button__text">{{ title }}</v-btn>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      typeof: String,
      require: true,
    },
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/utils";

.button {
  .button__link.button__link.button__link {
    margin-top: 40px;
    text-decoration: none;

    @include breakpoint(lg) {
      margin-top: 32px;
    }
  }

  .button__text.button__text.button__text {
    padding: 24px 20px;
    border-radius: 200px;
    background-image: linear-gradient(84deg, #f28b03, #f06500);
    font-family: $font_1;
    font-size: 16px;
    color: #fff;
    line-height: 26px;
    font-weight: 700;
    text-transform: capitalize;

    @include breakpoint(sm) {
      padding: 28px 20px;
      font-size: 18px;
    }
  }
}
</style>