<template>  
  <router-view :key="$route.fullPath"/>
  <!-- <el-button type="primary">我是按鈕</el-button> -->
</template>


<style>

#text {
  font-family: Helvetica;
  font-weight:bold;
}

#name {
  font-size: 50px;
  margin-block-start: 5px;
  margin-block-end: 10px;
  position: absolute;
  top: 20px;
  left: 55px;
  width: 200px;
  color:rgb(41, 117, 122);
}

.button1{
  padding-top: 0px;
  padding-left: 10px;
  border: none;
  color: white;
  display: inline-block;
}

main {
  margin: 0;
  width: 30vw;
}

body{
  background-color: rgb(157, 221, 224);
  margin: 0px; 
  /* 網頁的底色 */
}

</style>
