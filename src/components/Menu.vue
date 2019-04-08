<template>
  <div class="m-container">
    <div class="inner">
      <div v-for="item in menuData" v-bind:key="item.title" class="alpha">
        <button><h4 class="menuTitle" >{{item.title}}</h4></button>
        <div class="sub">
          <p v-for="subItem in item.sub" v-bind:key="subItem">{{subItem}}</p>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import MenuData from '../Utils/MenuData'
export default {
  name:'Menu',
  data(){
    return{
     menuData:MenuData
    }
  }

}
</script>

<style lang="scss" scopped>
  $menu-grey-dark : #EDECEC;
  $menu-grey-light:#F4F4F4;

  .m-container{
    width: 100%;
    height: 60px;
    background: white;
    position: relative;
    .inner{
      display: flex;
      height: 100%;
      align-items: center;
      justify-content: space-evenly;
      margin-right: 24px;
      
      
      .alpha{
        width: 120px;
        border-top-left-radius: 9px;
        border-top-right-radius: 9px;
        
      }

        .alpha:hover {
          background: $menu-grey-light;
          .sub{
            display: block;
            opacity: 1;

          }
        }

      button{
        width: 100%;
        height: 50px;
        border: none;
        background: transparent;
        padding:0;
        margin:0;
        position: relative;
       
        .menuTitle{
          font-size: 14px;
          text-transform: uppercase;
          line-height: normal;
          text-align: left;
          padding-left: 8px;
          }
      }
      .sub{
        position: absolute;
        background: $menu-grey-light;
        top:90%;
        opacity: 0;
        display: none;
        border-bottom-right-radius: 9px;
        border-bottom-left-radius: 9px;
        border-top-right-radius: 9px;
        overflow: hidden;
        transition: all 0.3s ease;
        z-index: 1000;
        
        p{
          display: block;
          text-align: left;
          font-size: 14px;
          width: 200px;
          padding: 8px;
          line-height: 16px;
          text-transform: uppercase; 

        }

        p:nth-child(even) {
          background:  $menu-grey-dark;
        }

        p:hover{
          cursor: pointer;
          color: $color-primary;
        }
      }

      
    }
  }
</style>
