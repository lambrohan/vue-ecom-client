<template>
  <div class="searchbar">
    <input type="text" placeholder="Search for products (diper, tops, jeans etc.)">
    <img src="../assets/ic_search.png" alt="">
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scooped >
.searchbar{
  margin-left: 30px;
  width: 450px;
  background: #fff;
  display: flex;
  align-items: center;
  padding: 2px;
  padding-left: 16px;
  border-radius: 10px;
  box-sizing: border-box;
  height: 34px;
  overflow: hidden;

  input{
    border: none;
    width: 90%;
    padding: 2px 8px;
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: normal;

  }

  img{
    width: 34px;
    height: 34px;
    padding: 8px;
    box-sizing: border-box;
  }
}
</style>
