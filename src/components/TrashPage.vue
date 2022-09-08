<template>
  <div id="trash-detail">
    <h1>{{ msg }}:{{ $route.params.noteId }}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "Trash page.",
    };
  },
};
</script>

<style scoped>
h1 {
  color: orange;
}
</style>