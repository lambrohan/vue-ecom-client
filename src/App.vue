<template>
  <div id="app">
    <Toolbar/>
    <div class="content">     
    <Menu/>
    <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Toolbar from '@/components/Toolbar';
import Menu from '@/components/Menu';
export default {
  name:'MyApp',
  components:{
    Toolbar,
    Menu
  }
}
</script>


<style lang="scss">
#app {
  font-family: 'Poppins', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  position: relative;
  width: 100%;
  z-index: 1;
}
.content{
  padding-top: 70px;
  position: relative;
  width: 100%;
  overflow: hidden;
  min-height: 100vh;
}

</style>
