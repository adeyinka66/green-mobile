<template>
  <div class="landingContainer">
    <nav-component></nav-component>
    <div class="circle1 position-absolute"><img :src="vector1" alt="" srcset="" width="75px" height="75px">  </div>
    <div class="circle2 position-absolute"><img :src="vector2" alt="" srcset="">  </div>
    <div class="circle3 position-absolute"><img :src="vector2" alt="" srcset="">  </div>
    <div class="circle4 position-absolute"><img :src="vector2" alt="" srcset="">  </div>
    <div class="circle5 position-absolute"><img :src="vector2" alt="" srcset="">  </div>
    <div class="circle6 position-absolute"><img :src="vector3" alt="" srcset="">  </div>


    <div class="d-flex justify-space-between align-center ma-container" >
      <div class="landingTextContainer">  <h2 class="atkinson-hyperlegible-bold">Experience The Future Of Mobile Technology</h2>
      <p>Exclusive Deals And Latest Models</p>
        <div class="d-flex justify-start ga-5 align-center maTop" >
          <div><img :src="arrow" alt="" srcset="">  </div>
          <div class="shopNow">  SHOP NOW </div>
        </div>
      </div>

      <div><img :src="phone1" alt="iphone" srcset="" width="429" height="605"> </div>
    </div>

  </div>
  <div class="section1" >

  </div>
</template>

<script setup>
import NavComponent from "@/components/navComponent.vue";
import vector1 from "../assets/img/circle1.svg"
import vector2 from "../assets/img/vector2.svg"
import phone1 from "../assets/img/phone1.png"
import arrow from "../assets/img/Arrow.png"
import vector3 from "../assets/img/vector2.svg"
</script>

<style lang="scss" scoped>
//@import '@/assets/scss/components/landing';
.landingContainer {
  width: 100%;
  height: 100vh;
  background: linear-gradient(180deg, #52B788 9.5%, rgba(82, 183, 136, 0.75) 31%, #52B788 57%, #306B50 78%, #000 100%);
  position: relative;
  .circle1 {
    position: absolute;
    top: 109px;
    left: 339px;
  }
  .circle2 {
    position: absolute;
    top: 229px;
    left: 128px;
  }
  .circle3 {
    position: absolute;
    top: 187px;
    left: 640px;
  }
  .circle4 {
    position: absolute;
    top: 412px;
    left: 810px;
  }
  .circle5 {
    position: absolute;
    top: 229px;
    left: 1200px;
  }
  .circle6 {
    position: absolute;
    top: 690px;
    left: 186px;
  }

  .landingTextContainer{
    width: 600px;
    //border: 1px solid red;
    h2 {
      color: #000;
      font-size: 54px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
    }
    p {
      color: #000;
      font-family: "Atkinson Hyperlegible", sans-serif;
      font-size: 36px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
    }
    .shopNow {
      color: #000;
      font-family: "Atkinson Hyperlegible", sans-serif;
      font-size: 36px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
    }
  }
}
.section1 {
  background: linear-gradient(180deg, #000 76%, #52B788 90.5%);
  width: 100%;
  height: 100vh;
}

</style>