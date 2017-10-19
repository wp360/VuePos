<template>
  <div id="app">
    <div class="header">
      <img src="./assets/logo.png">
      <p>欢迎进入Vue2.0 快餐店收银系统</p>
    </div>
    <leftNav></leftNav>
    <div class="main">
      <router-view/>
    </div>
  </div>
</template>

<script>
import leftNav from '@/components/common/leftNav'

export default {
  name: 'app',
  components: {
    leftNav
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.main{
  float: left;
  width: 95%;
  background-color: #EFF2F7;
  height: 100%;
  overflow: hidden;
}
.header{
  width: 100%;
  height: 40px;
  padding: 10px 0;
  background-color: white;
}
.header img{
  width: 30px;
  height: 30px;
  float: left;
  margin-left: 10%;
}
.header p{
  line-height: 40px;
  text-align: center;
  margin: 0;
}
</style>
