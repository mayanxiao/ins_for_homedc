<style>
*{
  padding: 0;
  margin: 0;
  text-decoration: none;
  list-style: none;
  box-sizing: border-box;
}
body{
  background: #f7f7f7;
}
.white-back {
  background-color: #fff;
}
input {
  outline: none;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>
<template>
  <div id="app">
    <nav-bar></nav-bar>
    <div class="mainbody">
      <router-view></router-view>
    </div>
    <!-- <j-footer></j-footer> -->
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'
import JFooter from '@/components/JFooter'

export default {
  name: 'app',
  components: {
    JFooter,
    NavBar
  }
}
</script>