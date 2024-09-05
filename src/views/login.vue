<template>
  <i-r-l-component :login="login" >
    <div class="hero_header_text inria-sans-bold d-flex flex-wrap justify-space-between align-center ga-5">

      <div class="email" >
        <label class="itim-regular d-block">Email Address</label>
        <div><input type="text" name="" id="" class="input-text-long"></div>
      </div>
      <div class="passsword">
        <label class="itim-regular d-block">Password</label>
        <div><input type="text" name="" id="" class="input-text-long"></div>
      </div>
      <div class="text-right "  style="visibility: hidden" >
        <button class="hero_btn"> Sign up </button>
      </div>
      <div class="text-right">
        <button class="hero_btn"> Sign up </button>
      </div>
    </div>

  </i-r-l-component>

</template>

<script setup>

import IRLComponent from "@/components/IRL-Component.vue";
import {ref} from "vue";

const login = ref('active')

</script>

<style lang="scss" scoped>
.hero_header_text {
  text-transform: uppercase;
  padding-top: 140px;
  width: 75%;
  margin: 0 auto;
  //border: 1px dotted blue;
  .email {
    width: 100%;
  }
  .passsword {
    width: 100%;
  }
  .fname {
    width: 45%;
  }
  .lname {
    width: 45%;
  }
  .input-text-short {
    width: 263px;
    height: 69px;
    flex-shrink: 0;
    border-radius: 23px;
    background: #D9D9D9;
  }
  .input-text-long {
    width: 600px;
    height: 69px;
    flex-shrink: 0;
    border-radius: 23px;
    background: #D9D9D9;
  }
}
label {
  color: #000;
  font-size: 18px;
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
  color: #52B788;
  text-transform: uppercase;
}
</style>