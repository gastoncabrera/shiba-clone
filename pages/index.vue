<template>
  <div>
    <Hero />

    <Ecosistem />

    <CoinsHome />

    <Buy />

    <Guide />

    <ShibaSwap />

    <Art />

    <Rescue />

    <Community />

    <SocialLinks />
  </div>
</template>

<script>
import Hero from "@/components/Home/Hero";
import Ecosistem from "@/components/Home/Ecosistem";
import CoinsHome from "@/components/Home/CoinsHome";
import Buy from "@/components/Home/Buy";
import Guide from "@/components/Home/Guide";
import ShibaSwap from "@/components/Home/ShibaSwap";
import Art from "@/components/Home/Art";
import Rescue from "@/components/Home/Rescue";
import Community from "@/components/Home/Community";
import SocialLinks from "@/components/Home/SocialLinks";

export default {
  components: {
    Hero,
    Ecosistem,
    CoinsHome,
    Buy,
    Guide,
    ShibaSwap,
    Art,
    Rescue,
    Community,
    SocialLinks,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
</style>
