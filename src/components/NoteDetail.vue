<template>
  <div id="note-detail">
    <h1>{{ msg }}:{{ $route.params.noteId }}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "Note detail page.",
    };
  },
};
</script>

<style scoped>
h1 {
  color: blue;
}
</style>