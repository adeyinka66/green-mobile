<template>
  <div class="ma-container">
  <div class="navContainer d-flex justify-space-between align-center" >
    <div class="navLogo"><img :src="logo" alt="" srcset=""  width="200px" height="85px"></div>
    <div class="d-flex justify-start align-center  navLinkContainer">
      <span><router-link to="" class="inria-sans-regular navLink">shop</router-link></span>
      <span> <router-link to="" class="inria-sans-regular navLink">about us</router-link> </span>
      <span> <router-link to="" class="inria-sans-regular navLink">contact</router-link> </span>
    </div>
    <div class="d-flex justify-space-around align-center navButton " >
      <div class="lr-button inria-sans-bold">  login / register </div>
    </div>
  </div>
  </div>
</template>

<script setup>
import logo from "../assets/img/logo.png"

</script>

<style lang="scss" scoped>
//@import '@/assets/scss/components/nav';
.navContainer {
  width: 100%;
  //border: 1px double orange;
  padding-top: 23px;
  .navLogo {
    width:20% ;
    border: 1px solid grey;
  }
  .navLinkContainer {
    width:60% ;
    //border: 1px dotted blue;
    padding: 0 40px;
    .navLink {
      color: #000;
      text-align: center;
      font-size: 18px;
      padding: 10px 20px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
      text-decoration: none;
      text-transform: uppercase;
    }
  }
  .navButton {
    width:15% ;
    border: 1px solid orange;
    .lr-button {
      width: 100%;
      flex-shrink: 0;
      border-radius: 39px;
      background: #fff;
      border: 1px solid #000;
      color: #000;
      text-align: center;
      font-style: normal;
      font-weight: 700;
      line-height: normal;
      text-transform: uppercase;
      cursor: pointer;
      font-size: 16px;
      padding: 10px 20px;
    }
  }

}

</style>