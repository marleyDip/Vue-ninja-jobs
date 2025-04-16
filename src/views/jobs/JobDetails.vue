<template>
  <div v-if="job">
    <h1>{{ job.title }}</h1>
    <h5>The job id is {{ id }}</h5>
    <h3>Name: {{ job.details.name }}</h3>
    <h4>Location: {{ job.details.location }}</h4>
    <h4>Salary: {{ job.details.salary }}</h4>
    <h4>Description: {{ job.details.description }}</h4>
  </div>

  <div v-else>
    <h3>Loading Job Details...</h3>
  </div>

  <!-- <p>The Job id is {{ $route.params.id }}</p> -->
</template>

<script>
export default {
  props: ["id"],
  /* data() {
    return {
      id: this.$route.params.id,
    };
  }, */
  data() {
    return {
      job: null,
    };
  },
  mounted() {
    //fetch(`http://localhost:3000/jobs/${this.$route.params.id}`)
    fetch("http://localhost:3000/jobs/" + this.id)
      .then((res) => res.json())
      .then((data) => (this.job = data))
      .catch((err) => console.log(err.message));
  },
};
</script>

<style>
</style>