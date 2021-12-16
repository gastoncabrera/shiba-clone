<template>
  <div>
    <div class="guide__wrap">
      <div class="guide__left">
        <div class="guide__id">
          <div class="guide__id_number">{{ id }}</div>
        </div>
        <div class="guide__line"></div>
      </div>
      <div class="guide__right">
        <h3 class="guide__title_wrap">{{ title }}</h3>
        <p class="guide__description_wrap">
          {{ description }}
        </p>
      </div>
    </div>
    <div class="guide__line_divider" v-show="show"></div>
  </div>
</template>

<script>
export default {
  props: {
    id: {
      typeof: Number,
      require: true,
    },

    title: {
      typeof: String,
      require: true,
    },

    description: {
      typeof: String,
      require: true,
    },

    show: {
      typeof: Boolean,
      default: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

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