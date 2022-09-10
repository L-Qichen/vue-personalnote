<template>
  <div :title="user.username">{{ slug }}</div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        username: "Toby",
      },
      slug: "t",
    };
  },
};
</script>

<style scoped>
div {
  margin: 0px auto;
  width: 36px;
  height: 36px;
  text-align: center;
  line-height: 36px;
  font-size: 18px;
  font-weight: bold;
  border-radius: 50%;
  background: #f2b81c;
  color: #fff;
  text-shadow: 1px 0 1px #795c19;
  margin-top: 16px;
  margin-bottom: 16px;
  text-transform: uppercase;
}
</style>