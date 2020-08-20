<template>
  <div>

    <button v-on:click="upFunction" class="btn btn-info">{{lable}}</button>
     <button v-on:click="downFunction" class="btn btn-info">{{lable}}</button>
    <p v-bind:style="{fontSize:fsize + 'px'}" >HELLO {{counter}}</p>
  </div>
</template>

<script>
export default {
    data: function() {
        return {
            counter: 0,
            fsize:50

        }
    },

  props: {
    lable: String,
  },
  methods: {
      upFunction: function(){
          // eslint-disable-next-line no-undef
          this.counter += 1;
          // eslint-disable-next-line no-undef
          this.fsize += 10;

          //console.log('fsize ='+this.fsize);
          //console.log('counter = '+this.counter);
          //ส่งค่าตัวแปร counter ออกไปโดยผ่านตัวแปร cc
          this.Semit('cc', this.counter)
          
      },
       downFunction: function(){
          // eslint-disable-next-line no-undef
          this.counter -= 1;
          // eslint-disable-next-line no-undef
          this.fsize -= 10;

          console.log(this.fsize);
          console.log(this.counter);
      },
  },



}




</script>

<style>

</style>
