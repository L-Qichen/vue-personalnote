<template>
  <div id="app">
    <sidebar />
    <router-view />
  </div>
</template>

<script>
import sidebar from "@/components/SideBar.vue";

export default {
  name: "App",
  components: {
    sidebar,
  },
};
</script>

<style>
@import "//at.alicdn.com/t/font_496303_kqrjhri8l25d0a4i.css";

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

*::before {
  box-sizing: border-box;
}

*::after {
  box-sizing: border-box;
}

html,
body,
#app {
  height: 100%;
}

body {
  font-family: "Avenir", Arial, Helvetica, sans-serif;
  font-size: 14px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #eee;
}

a {
  text-decoration: none;
  color: #444;
}

ul,
ol {
  list-style: none;
}

#app {
  display: flex;
}
</style>
