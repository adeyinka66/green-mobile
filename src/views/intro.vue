<template>
  <div  class="d-flex justify-space-between align-center l-container" >
    <div class="ellipse_360"></div>
    <div class="ellipse_361"></div>
    <div class="ellipse_362"></div>
     <div class="w-30 ls1 ">
       <img :src="logo" alt="" srcset="">
       <div class="landing_options_cover">
         <router-link :to="{name:'intro'}" class="text-decoration-none"><div class="intro_btn active  itim-regular" > intro </div></router-link>
         <router-link :to="{name: 'register'}" class="text-decoration-none"> <div class="intro_btn  itim-regular"  >sign up</div></router-link>
         <router-link :to="{name: 'login'}"  class="text-decoration-none"> <div class="intro_btn itim-regular" > login</div> </router-link>
       </div>

     </div>
    <div class="w-70 ls2"  >
      <div class="ellipse w-100">
        <div class="hero_header_text inria-sans-bold">Welcome!</div>
        <div class="hero_text inria-sans-regular">
          your one-stop destination for premium  <span style="color: red">phone repairs</span> , <span style="color: red">phone accessories</span> , and <span style="color: red">covers</span> . Experience exceptional service and quality products tailored to meet all your mobile needs.
        </div>
       <div class="text-center">
         <button class="hero_btn"> Sign up </button>
       </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import  logo from "../assets/img/logo.png"
</script>

<style lang="scss" scoped>
.l-container {
  position: relative;
  .ellipse_360 {
    border-radius: 50%;
    position: absolute;
    width: 268.842px;
    height: 268.842px;
    transform: rotate(202.057deg);
    flex-shrink: 0;
    background: #B7E4C7;
    filter: blur(500px);
    left: 210px;
    transition: 1s;
    z-index: -5 !important;
  }
  .ellipse_360:hover {
    background: red;
    transform: translate(0, 200px) rotate(360deg);
  }
  .ellipse_361 {
    position: absolute;
    border-radius: 50%;
    background: #74C69D;
    filter: blur(200px);
    width: 268.842px;
    height: 268.842px;
    transform: rotate(102.057deg);
    flex-shrink: 0;
    left: 300px;
    top: 210px;
  }
  .ellipse_362 {
    width: 345px;
    height: 345px;
    flex-shrink: 0;
    border-radius: 50%;
    background: #B7E4C7;
    filter: blur(200px);
    position: absolute;
    left: 600px;
    top: 290px;
  }
  .ls1 {
    //border: 1px dotted green;
    width: 35%;
    height: 100vh;
    .landing_options_cover {
      //border: 2px dotted blue;
      width: 200px;
      margin-left: 180px;
      .intro_btn {
        width: 400px;
        height: 101px;
        padding: 12px 24px;
        flex-shrink: 0;
        border-radius: 77px;
        color: #000;
        font-size: 60px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        text-transform: uppercase;
        margin-bottom: 4%;
        cursor: pointer;
      }
      .active {
        background: #52B788;
      }
    }
  }
  .ls2{
    //border: 1px dotted red;
    width: 65%;
    height: 100vh;
    .ellipse {
      background-image: url("../assets/img/landing-bg.png");
      background-repeat: no-repeat;
      background-size: 100% 110%;
      background-position: center;
      background-blend-mode: color-burn;
      height: 100vh;
      padding: 20px;
      .hero_header_text {
        color: #000;
        text-align: center;
        font-size: 96px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        text-transform: uppercase;
        padding-top: 120px;
      }
      .hero_text {
        width: 600px;
        margin: 0 auto;
        border: 1px dotted orange;
        color: #000;
        text-align: center;
        font-size: 26px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        text-transform: uppercase;
      }
      .hero_btn {
        width: 243px;
        height: 69px;
        flex-shrink: 0;
        border-radius: 23px;
        background: #FFF;
        text-align: center;
        font-size: 36px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        color: #111;
        margin-top: 5%;
      }
    }
  }
}



</style>