<template>
  <div id="sidebar">
    <avatar />
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
import avatar from "@/components/Avatar";

export default {
  components: {
    avatar,
  },
  methods: {
    onLogout() {},
  },
};
</script>

<style lang="less" scoped>
#sidebar {
  position: relative;
  width: 68px;
  text-align: center;
  background-color: #2c333c;

  a {
    padding: 12px 0;
    display: block;
  }

  .router-link-active {
    background-color: #5e6266;
  }
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