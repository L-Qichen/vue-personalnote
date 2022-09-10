<template>
  <div id="sidebar">
    <div class="icons">
      <router-link to="/note/1">
        <div class="iconfont icon-note">icon</div>
      </router-link>
      <router-link to="/notebooks">
        <div class="iconfont icon-notebook">icon</div>
      </router-link>
      <router-link to="/trash/2">
        <div class="iconfont icon-trash">icon</div>
      </router-link>
      <div class="logout">
        <button class="iconfont icon-logout" @click="onLogout">icon</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {},
};
</script>

<style scoped>
#sidebar {
  border: 1px solid red;
}
#sidebar > div .iconfont {
  border: 1px solid orange;
}
.logout {
  border: 1px solid blue;
}
</style>