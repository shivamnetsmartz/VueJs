<template>
  <div>
    <h1>Hello World from Home Component</h1>
    <!-- <h1>{{ data }}</h1>
    <h1>{{ msg }}</h1> -->
    <button v-on:click="View">Call View function</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String,
  },
  methods: {
    View() {
      alert("View function called ");
    },
  },
};
</script>

<style>
h1 {
  background-color: rgb(59, 190, 118);
  color: white;
}
</style>
