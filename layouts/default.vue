<template>
  <v-app color="white">
    <TopBar />
    <v-main app>
      <Nuxt />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";
AOS.init();
export default {
  data() {
    return {
      filterParams: false,
    };
  },
  head: {
    script: [
      {
        src: "/scripts/jquery-3.3.1.min.js",
        type: "text/javascript",
        body: true,
      },
    ],
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
</style>