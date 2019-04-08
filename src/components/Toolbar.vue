<template>
 <div class="t-container">
    <div class="toolbar">
    <div class="branding">
      <img src="../assets/logo.png" alt="">
    </div>
    <Searchbar/>
  </div>
 
 </div>
</template>

<script>
import Searchbar from './Searchbar'


export default {
  components:{
    Searchbar,
  }

}
</script>
<style lang="scss" scopped>
.t-container{
  z-index: 1000;
  position: fixed;
  width: 100%;
}

.toolbar{
  width: 100%;
  height:70px;
  background:$color-primary;
  display: flex;
  align-items: center;

  .branding{
    margin-left: 3rem; 
    height: 100%;
    img{
      height: 100%;
      padding: 4px;
      box-sizing: border-box;
    }
  }
}

</style>
