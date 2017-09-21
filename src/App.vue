<template>
  <div id="app">
    <img class="logo" src="./assets/logo.svg">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app',
};
</script>

<style>
.logo {
  width: 200px;
  height: 200px;
  float: right;
  margin-right: 6em;
}

body {
  font-family: Menlo, Consolas, monospace;
  color: #444;
}

</style>
