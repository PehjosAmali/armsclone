<template lang="">
    <div class="vue">
    <p> this is the best demo app from vue</p>
<h2>{{name}}</h2>
<h2>{{age}}</h2>
<p @click="increment">{{count}}</p>
<p @click="decrement">{{count}}</p>
<p>{{this.hello}}</p>
<button @click="handleClick">CLICK ME</button>
    </div>
</template>
<script>
export default {
    name:"DemoItem",
    props:{
name:String,
age:String,


    },
    data() {
    return {
      count: 0,
      hello:"peh"
    }
  },
    methods:{
handleClick(){

    alert("hellow")
},
increment() {
      this.count++
    }
,
decrement() {
      this.count--
    }
    },
    mounted() {
    console.log(`the component is now mounted.`)
  },




}
</script>
<style  scoped>
 .vue>p{
color: red;


 }
</style>