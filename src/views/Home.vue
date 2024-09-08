<template>
  <div class="landingContainer">
    <nav-component></nav-component>
    <div class="circle1 position-absolute" v-for="item in bubble" :key="item.sn" :style="{top: item.top, left:item.left}" ><img :src="vector1" alt="vector1" srcset="" :width="item.width" :height="item.height">  </div>

    <div class="d-flex justify-space-between align-center ma-container" style="padding: 50px 0" >
      <div class="landingTextContainer">  <h2 class="atkinson-hyperlegible-bold">Experience The Future Of Mobile Technology</h2>
      <p>Exclusive Deals And Latest Models</p>
        <div class="d-flex justify-start ga-3 align-center maTop" >
          <div><img :src="arrow" alt="" srcset="" width="24px">  </div>
          <div class="shopNow">  SHOP NOW </div>
        </div>
      </div>

      <div><img :src="phone1" alt="iphone" srcset="" width="400" height="550"> </div>
    </div>

  </div>
  <div class="section1" >
    <div class="d-flex justify-space-between align-center ma-container">
      <div class="smallDots d-flex justify-center align-center" >
        <div class="phoneBackground align-self-center" >
          <img :src="phone2" alt="" srcset=""  width="430.621px"  height="410.317px">
        </div>
      </div>

      <div class="section1Text-container">
        <div class="protect atkinson-hyperlegible-bold">
           <h2>Protect your phone in style with our premium, durable, and trendy covers </h2>
          <p>because your phone deserves the best.</p>
        </div>
        <div class="d-flex justify-start align-center ga-5 maTop">
          <div class="explore">Explore More</div>
          <div><svg xmlns="http://www.w3.org/2000/svg" width="24" height="16" viewBox="0 0 50 16" fill="none" stroke="#52B788" stroke-width="3px">
            <path d="M34 8C34 12.4183 37.5817 16 42 16C46.4183 16 50 12.4183 50 8C50 3.58172 46.4183 0 42 0C37.5817 0 34 3.58172 34 8ZM0 9.5L42 9.5V6.5L0 6.5L0 9.5Z" fill="#52B788"/>
          </svg></div>
        </div>
      </div>
    </div>

  </div>
  <div class="section2">
   <div class="ma-container d-flex justify-space-between align-center">
     <div class="section2Text-container">
       <div class="protect atkinson-hyperlegible-bold">
          <h2 class="sectionTextH">Get your phone fixed quickly and affordably at our shop.</h2>
         <p class="sectionTextP">where expert technicians ensure top-quality repairs and customer satisfaction.</p>
       </div>
       <div class="d-flex justify-start align-center ga-5 maTop">
         <div class="explore sectionTextB">Explore More</div>
         <div><svg xmlns="http://www.w3.org/2000/svg" width="24" height="16" viewBox="0 0 50 16" fill="none" stroke="#fff" stroke-width="3px">
           <path d="M34 8C34 12.4183 37.5817 16 42 16C46.4183 16 50 12.4183 50 8C50 3.58172 46.4183 0 42 0C37.5817 0 34 3.58172 34 8ZM0 9.5L42 9.5V6.5L0 6.5L0 9.5Z" fill="#52B788"/>
         </svg></div>
       </div>
     </div>
     <div><img :src="phone3" alt="" srcset="" width="550px" height="470px"></div>
   </div>
  </div>
  <div class="section3">
    <div class="ma-container d-flex justify-space-between align-center">
      <div><img :src="iwatch" alt="" srcset=""></div>
      <div class="section3Text-container">
        <div class="protect atkinson-hyperlegible-bold">
           <h2 class="sectionTextH">Upgrade your phone with our top-notch accessories.</h2>
          <p class="sectionTextP">combining quality, style, and functionality – all available at unbeatable prices.</p>
        </div>
        <div class="d-flex justify-start align-center ga-5 maTop">
          <div class="explore sectionTextB" >Explore More</div>
          <div class=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="16" viewBox="0 0 50 16" fill="none" stroke="#52B788" stroke-width="3px">
            <path d="M34 8C34 12.4183 37.5817 16 42 16C46.4183 16 50 12.4183 50 8C50 3.58172 46.4183 0 42 0C37.5817 0 34 3.58172 34 8ZM0 9.5L42 9.5V6.5L0 6.5L0 9.5Z" fill="#52B788"/>
          </svg></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import NavComponent from "@/components/navComponent.vue";
import vector1 from "../assets/img/circle1.svg"
import phone1 from "../assets/img/phone1.png"
import phone2 from "../assets/img/phone2.png"
import phone3 from "../assets/img/phone3.png"
import iwatch from "../assets/img/watch.png"
import arrow from "../assets/img/Arrow.png"
import { ref } from 'vue'


const bubble = ref([
  {width: '75px', height: '75px',top: '150px', left: '280px', sn: 1},
  {width: '42px', height: '42px',top: '240px', left: '38px', sn: 2},
  {width: '40px', height: '40px',top: '287px', left: '640px', sn: 3},
  {width: '54px', height: '54px',top: '329px', left: '1200px', sn: 4},
  {width: '35px', height: '35px',top: '690px', left: '66px', sn: 5},
  {width: '45px', height: '45px',top: '821px', left: '473px' , sn: 6},
])

</script>

<style lang="scss" scoped>
//@import '@/assets/scss/components/landing';
.landingContainer {
  width: 100%;
  height: auto;
  background: linear-gradient(180deg, #52B788 9.5%, rgba(82, 183, 136, 0.75) 31%, #52B788 57%, #306B50 78%, #000 100%);
  position: relative;
  .circle1 {
    position: absolute;
    top: 109px;
    left: 339px;
  }

  .landingTextContainer{
    width: 600px;
    //border: 1px solid red;
    padding: 0 10px;
    h2 {
      color: #000;
      font-size: 50px;
      font-style: normal;
      font-weight: 550;
      line-height: normal;
    }
    p {
      color: #000;
      font-family: "Atkinson Hyperlegible", sans-serif;
      font-size: 24px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
    }
    .shopNow {
      color: #000;
      font-family: "Atkinson Hyperlegible", sans-serif;
      font-size: 18px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
      border: 2px solid #000;
      padding: 10px;
      cursor: pointer;
      border-radius: 20px;
      transition: box-shadow 0.3s ease;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1), /* bottom shadow */
      0 -4px 6px rgba(0, 0, 0, 0.05), /* top shadow */
      4px 0 6px rgba(0, 0, 0, 0.05), /* right shadow */
      -4px 0 6px rgba(0, 0, 0, 0.05); /* left shadow */
    }
    .shopNow:hover {
      box-shadow: 0 6px 10px rgba(0, 0, 0, 0.15),
      0 -6px 10px rgba(0, 0, 0, 0.1),
      6px 0 10px rgba(0, 0, 0, 0.1),
      -6px 0 10px rgba(0, 0, 0, 0.1);
    }
  }
}
.section1 {
  background: linear-gradient(180deg, #000 76%, #52B788 90.5%);
  width: 100%;
  height: auto;
  padding: 200px 0;
  .smallDots {
    //border: 1px solid purple;
    width: 535.018px;
    height: 500.96px;
    flex-shrink: 0;
    background-image: url("../assets/img/smalldots.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    .phoneBackground {
      width: 380.592px;
      height: 390.882px;
      flex-shrink: 0;
      background-image: url("../assets/img/phonebackground.png");
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
    }
  }
  .section1Text-container {
    width: 644px;
    //border: 1px dotted yellow;
    .protect {
      color: #FFF;
      h2 {
        color: #fff;
        font-size: 45px;
        font-style: normal;
        font-weight: 550;
        line-height: normal;
        font-family: "Atkinson Hyperlegible", sans-serif;
      }
      p {
        color: #fff;
        font-family: "Atkinson Hyperlegible", sans-serif;
        font-size: 24px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        text-transform: capitalize;
        margin-top: 3%;
      }
    }
    .explore {
      color: #52B788;
      text-align: center;
      font-family: "Atkinson Hyperlegible", sans-serif;
      line-height: normal;
      font-size: 18px;
      font-style: normal;
      font-weight: 600;
      //border: 2px solid #52B788;
      padding: 10px;
      cursor: pointer;
      border-radius: 20px;
      transition: box-shadow 0.3s ease;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1), /* bottom shadow */
      0 -4px 6px rgba(0, 0, 0, 0.05), /* top shadow */
      4px 0 6px rgba(0, 0, 0, 0.05), /* right shadow */
      -4px 0 6px rgba(0, 0, 0, 0.05); /* left shadow */
    }
    .explore:hover {
      box-shadow: 0 6px 10px rgba(0, 0, 0, 0.15),
      0 -6px 10px rgba(0, 0, 0, 0.1),
      6px 0 10px rgba(0, 0, 0, 0.1),
      -6px 0 10px rgba(0, 0, 0, 0.1);
    }
  }
}
.section2 {
  width: 100%;
  height: auto;
  background: linear-gradient(180deg, #52B788 9.5%, rgba(82, 183, 136, 0.75) 31%, #52B788 57%, #306B50 78%, #000 100%);
  padding-bottom: 120px;
  .section2Text-container {
    width: 644px;
    //border: 1px dotted purple;
    .protect {
      color: #FFF;
      h2 {
        color: #000;
        font-family: "Atkinson Hyperlegible", sans-serif;
      }
      p {
        color: #000;
      }
    }
    .explore {
      color: #fff;
      text-align: center;
      border: 2px solid #fff;
      font-family: "Atkinson Hyperlegible", sans-serif;
    }
  }
}
.section3 {
  width: 100%;
  height: 100vh;
  background: linear-gradient(180deg, #000 76%, #52B788 90.5%);
  padding: 100px 0;
  .section3Text-container {
    width: 644px;
    //border: 1px dotted brown;
    .protect {
      color: #FFF;
      h2 {
        color: #fff;
      }
      p {
        color: #fff;
      }
    }
    .explore {
      color: #52B788;
      border: 2px solid #52B788;
      text-align: center;
      font-family: "Atkinson Hyperlegible", sans-serif;
    }
  }

}

</style>