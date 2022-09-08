<template>
  <div id="notebook-list">
    <h1>{{ msg }}</h1>
    <ul>
      <li><router-link to="/note/1">The first notebook.</router-link></li>
      <li><router-link to="/note/2">The second notebook.</router-link></li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "The Notebook list is displayed on this page.",
    };
  },
};
</script>

<style scoped>
h1 {
  color: red;
}
</style>