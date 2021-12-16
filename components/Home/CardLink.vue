<template>
  <div class="card_link">
    <div class="card_link__wrap">
      <img :src="imgBg" alt="" class="card_link__image_hover" />

      <img :src="img" alt="" class="card_link__image" />
    </div>

    <div class="card_link__text">{{ text }}</div>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      typeof: String,
      require: true,
    },

    imgBg: {
      typeof: String,
      require: true,
    },

    img: {
      typeof: String,
      require: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.card_link {
  display: flex;
  align-items: center;
  padding: 24px;
  margin: 10px 0;
  border-radius: 16px;
  background-color: #18171f;

  @include breakpoint(sm) {
    width: 190px;
    padding: 24px 32px;
    flex-direction: column;
    margin: 10px;
  }
}

.card_link__image_hover {
  display: none;
}

.card_link__image {
  width: 60px;
  height: 60px;
  object-fit: cover;
}

.card_link__text {
  margin-left: 24px;
  color: #bbbbbe;
  font-family: $font_1;
  font-size: 16px;
  line-height: 24px;
  text-align: center;

  @include breakpoint(sm) {
    margin-left: 0;
  }

  @include breakpoint(xl) {
    margin-left: 0;
  }
}
</style>