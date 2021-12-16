<template>
  <v-app app>
    <Banner />
    <Header />
    <v-main>
      <Nuxt />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Footer from "@/components/Layout/Default/Footer";
import Banner from "@/components/Layout/Default/Banner";
import Header from "@/components/Layout/Default/Header.vue";

export default {
  components: {
    Footer,
    Banner,
    Header,
  },
};
</script>
