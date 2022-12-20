<template>
  <SearchFilter :type="$route.params.type" />
</template>

<script>
export default {
  layout: "property",
  mounted() {
    console.log(this.$route.params.type);
  },
};
</script>

<style lang="scss" scoped>
</style>