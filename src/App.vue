<template>
 <div id="app">
    <HelloWorld msg="ARAYA TARIN" />
    <hr>
    <div class="row">
      <div class="col-6">
   
        <h1>{{total1}}</h1>
      </div>
      <div class="col-6">

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
}
</style>