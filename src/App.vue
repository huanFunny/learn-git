<!--
 * @Description: 文件描述
 * @Author: 洛欢
 * @Date: 2022-04-13 17:36:04
 * @LastEditTime: 2022-04-16 18:16:31
 * @LastEditors: 洛欢
-->
<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
input {
  width: 200px;
  height: 34px;
  line-height: 34px;
  font-size: 16px;
}
</style>
