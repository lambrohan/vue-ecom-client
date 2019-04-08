<template>
  <div id="c-container">
    <div class="slide"></div>
    <div class="btn left">
      <img src="../assets/ic_arrow_left.png" alt="">
    </div>
    <div class="btn right">
       <img src="../assets/ic_arrow_right.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name:"Carousel",
  data(){
    return{

    }
  }

}
</script>

<style lang="scss" scopped>
#c-container{
  width: 100%;
  height: 365px;
  position: relative;
  overflow: hidden;

  .slide{
    background-image: url('../assets/carousel-demo.png');
    position: absolute;
    width: 100%;
    height: 100%;

  }

  .btn{
    width: 84px;
    height: 84px;
    border-radius: 50%;
    background: #ffffff;
    position: absolute;
    cursor: pointer;

    img{
      width: 19px;
      height: 19px; 
      position: absolute;
      transform: translateY(-50%);
    }
  }

  .left{
    top:50%;
    transform: translate(-50%,-50%);
    img{
      top:50%;
      right:20%;
    }
  }

  .right{
    top:50%;
    right:0;
    transform: translate(50%,-50%);
   img{
     left:20%;
     top:50%;
   }
  }
}
</style>
