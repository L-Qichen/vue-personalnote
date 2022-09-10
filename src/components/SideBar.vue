<template>
  <div id="sidebar">
    <div class="icons">
      <router-link to="/note/1">
        <div class="iconfont icon-note"></div>
      </router-link>
      <router-link to="/notebooks">
        <div class="iconfont icon-notebook"></div>
      </router-link>
      <router-link to="/trash/2">
        <div class="iconfont icon-trash"></div>
      </router-link>
      <div class="logout" @click="onLogout">
        <div class="iconfont icon-logout"></div>
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
  position: relative;
  width: 68px;
  text-align: center;
  background-color: #2c333c;
}

.icons {
  margin-top: 15px;
}

.icons a {
  padding: 6px 0;
  display: block;
}

.icons .router-link-active {
  background-color: #5e6266;
}

.logout {
  position: absolute;
  bottom: 36px;
  width: 100%;
  text-align: center;
  cursor: pointer;
}

.iconfont {
  color: #fff;
}
</style>