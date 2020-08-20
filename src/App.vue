<template>
 <div id="app">
  <img alt="Vue logo" src="./assets/logo.jpg" />
    <HelloWorld msg="Thawatchai" />
    <hr>
    <div class="row">
      <div class="col-6">
    <img alt="Vue logo" src="https://thelistlove.com/wp-content/uploads/2015/07/Royal-Flush.gif" width="500" height="281" />
        <h1>{{total1}}</h1>
      </div>
      <div class="col-6">

<img alt="Vue logo" src="https://media0.giphy.com/media/3oeHLrjZGBgnPx5VII/giphy.gif" />
        <h1>{{total2}}</h1>
      </div>
      <div class="col-6">
        <CsButton @cc="sum" />
      </div>
      <div class="col-6">
        <CsButton @cc="sum1" />
      </div>
    </div>
    
  </div>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import CsButton from "./components/CSButton.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    CsButton,
    
  },
  data : function(){
    return {
    total1: 0,
    total2: 0,
   
   } 
  },
  methods: {
  sum(counterValue){
    this.total1 = counterValue
  },
  
  sum1(counterValue){
    this.total2 = counterValue
 
  
},
},

};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0b44ff;
  margin-top: 60px;
  background: url(https://images.wallpapersden.com/image/download/line-colorful-bright_4075_2560x1600.jpg) no-repeat center fixed;
  background-size: cover;
}
</style>