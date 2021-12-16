<template>
  <div class="coin">
    <div class="box_coin__top">
      <div class="box_coin__image_container">
        <img :src="img" alt="" class="box_coin__image_coin" />

        <img src="coin-shad-1.png" alt="" class="box_coin__image_shadow" />
      </div>
    </div>

    <div class="box_coin__bottom">
      <div class="box_coin__wrap_title">
        <h3 class="box_coin__title">{{ title }}</h3>

        <div class="box_coin__box_graph">
          <img src="ico-graph-ora.svg" alt="" class="box_coin__grap_image" />

          <p class="box_coin__grap_title">See Live Charts</p>
        </div>
      </div>

      <slot name="description"></slot>

      <Btn :title="title" />
    </div>
  </div>
</template>

<script>
import Btn from "@/components/Shared/Btn";

export default {
  components: {
    Btn,
  },

  props: {
    title: {
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

.coin {
  overflow: hidden;
  border-radius: 16px;
}

.box_coin__top {
  height: 100%;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  padding-top: 50px;
  padding-bottom: 100px;
  background: #191920;
  background: -webkit-linear-gradient(to right, #191920, #1f1e29);
  background: linear-gradient(to right, #191920, #1f1e29);
}

.box_coin__image_container {
  position: relative;
  height: 100px;
  width: 100px;
  margin: 0 auto;
}

.box_coin__image_coin {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 10;
}

.box_coin__image_shadow {
  position: absolute;
  bottom: -100px;
  left: -100px;
}

.box_coin__bottom {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #18171f;
  padding: 32px 32px 40px;

  @include breakpoint(sm) {
    align-items: flex-start;
  }
}

.box_coin__wrap_title {
  @include breakpoint(sm) {
    display: flex;
    align-items: center;
    margin-bottom: 14px;
  }
}

.box_coin__title {
  font-family: $font_1;
  font-size: 24px;
  line-height: 35px;
  color: white;
  text-align: center;
  margin-right: 32px;

  @include breakpoint(sm) {
    font-size: 30px;
    line-height: 42px;
  }
}

.box_coin__box_graph {
  display: flex;
  align-items: flex-start;
  padding: 10px;
  background-color: #24222e;
  margin-top: 10px;
  margin-bottom: 24px;
  padding: 8px 16px 3px;
  border-radius: 4px;
}

.box_coin__grap_image {
  margin-right: 5px;
}

.box_coin__grap_title {
  font-family: $font_1;
  font-size: 12px;
  color: white;
  font-weight: 700;
  margin: 0;
  padding: 0;
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
</style>

<style lang="scss">
@import "@/assets/scss/utils";

.box_coin {
  .box_coin__buttom_container {
    margin-top: 40px;
    text-decoration: none;

    @include breakpoint(lg) {
      margin-top: 32px;
    }
  }

  .box_coin__buttom_text {
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
      padding: 32px 24px;
      font-size: 18px;
    }
  }
}
</style>