<template>
  <div>
    <h1>{{ studentname }}</h1>
    <p v-html="htmltest"></p>
    <p>{{ htmltest }}</p>
  </div>
</template>

<script>
export default {
  name: "DemoComponent",
  data() {
    return {
      studentname: "Stefan",
      age: 34,
      htmltest: "<b>This is bold<b>",
    };
  },
  props: {
    message: String,
  },
  methods: {
    doSomething() {
      alert(this.studentname);
    },
  },
  mounted() {
    alert("Fully loaded!");
  },
};
</script>

<style>
</style>