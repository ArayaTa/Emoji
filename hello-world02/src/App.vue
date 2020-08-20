<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <h1>{{total}}</h1>
    <div class="row">
      <div class="col-3">
        <!--2.รับค่าจาก emit @cc แล้วส่งไป-->
        <Counter lable="ok" @cc="sum" />
      </div>
      <div class="col-3">
        <Counter lable="lol" @cc="sum" />
      </div>
      <div class="col-3">
        <Counter lable="Cancle" @cc="sum" />
      </div>
      <div class="col-3">
        <Counter lable="Yep" @cc="sum" />
      </div>
    </div>
    ชื่อ-นามสกุล <input type="text" v-model="name">
    รหัสนศ.  <input type="text" v-model="code">
    GPA  <input type="number" v-model="gpa" step="0.01">
    <hr/> 
    แสดงชื่อ + รหัสนศ+GPA
    {{name}} {{code}} {{gpa}}
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Counter from "./components/Counter.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Counter,
  },

  data: function () {
    return {
      total: 0, // ผลรวมทั้งหมด เาไปแสดงผล {{}}
      name:'',
      code:'',
      gpa:0.0,
    };
  },

  methods: {
    //3. คำนวนจากผลรวมทั้งหมดที่สงออกมาจาก emit แล้วเก็บผลรวมไว้ที่นี่ this.total
    sum(CounterValue) {
      this.total += CounterValue;
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
  color: #2c3e50;
  margin-top: 60px;
}
</style>
