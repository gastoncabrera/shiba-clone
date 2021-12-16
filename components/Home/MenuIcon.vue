<template>
  <div class="wrap">
    <div class="menu" @click="DropdawnMenu">
      <div
        :class="!close ? 'menu__linear' : 'menu__linear menu__linear--one'"
      ></div>
      <div
        :class="!close ? 'menu__linear' : 'menu__linear menu__linear--two'"
      ></div>
      <div
        :class="!close ? 'menu__linear' : 'menu__linear menu__linear--three'"
      ></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      close: false,
    };
  },

  methods: {
    DropdawnMenu() {
      this.$emit("Dropdawn");
      this.close = !this.close;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.wrap {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 30;
  padding-right: 32px;

  @include breakpoint(lg) {
    padding-right: 64px;
  }
}

.menu {
  display: block;
  cursor: pointer;
  position: relative;
  height: 35px;
  width: 35px;

  @include breakpoint(xl) {
    display: none;
  }
}

.menu__linear {
  transition: 300ms linear;
  height: 3px;
  background-color: white;
  width: 100%;
  margin-top: 7px;
  margin-bottom: 7px;
  border-radius: 200px;
}

.menu__linear--one {
  transition: 250ms linear;
  transform: rotate(45deg);
  position: absolute;
  margin-top: 17px;
}

.menu__linear--two {
  transition: 30ms linear;
  background-color: transparent;
}

.menu__linear--three {
  transition: 250ms linear;
  transform: rotate(-45deg);
  position: absolute;
}
</style>