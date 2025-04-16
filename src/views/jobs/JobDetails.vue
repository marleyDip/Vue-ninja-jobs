<template>
  <h1>Job Details Pages</h1>
  <!-- <p>The Job id is {{ $route.params.id }}</p> -->
  <p>The job id is {{ id }}</p>
</template>

<script>
export default {
  props: ["id"],
  /* data() {
    return {
      id: this.$route.params.id,
    };
  }, */
};
</script>

<style>
</style>