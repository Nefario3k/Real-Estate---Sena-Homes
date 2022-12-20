<template>
  <v-app dark style="background: var(--secondary-color)">
    <v-main app class="main">
      <v-container class="containedError">
        <h1 v-if="error.statusCode === 404">
          {{ error.statusCode }}
          <br />
          {{ pageNotFound }}
        </h1>
        <h1 v-else>
          {{ otherError }}
        </h1>
        <NuxtLink to="/"> Home page </NuxtLink>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "EmptyLayout",
  layout: "empty",
  props: {
    error: {
      type: Object,
      default: null,
    },
  },
  data() {
    return {
      pageNotFound: "Page Not Found",
      otherError: "An error occurred",
    };
  },
  head() {
    const title =
      this.error.statusCode === 404 ? this.pageNotFound : this.otherError;
    return {
      title,
    };
  },
};
</script>

<style scoped lang="scss">
.containedError {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;

  h1 {
    font-size: 370%;
    color: var(--primary-color);
    text-align: center;
    margin-bottom: 30px;
  }
  a {
    text-transform: none;
    text-decoration: none;
    color: #fff;
  }
}
</style>
