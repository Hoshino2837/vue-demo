<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>  -->
  <!-- <if20250818/> -->
  <!-- <forms/> -->
  <!-- <process/> -->
  <!-- <model/> -->
   <props :message="message" :age="age" :name="name"/>
</template>

<script>
  // import HelloWorld from './components/HelloWorld.vue',
  // import if20250818 from './components/条件渲染20250818.vue'
  // import forms from './components/forms20250819.vue'
  // import process from './components/事件处理20250819.vue'
  // import model from './components/表单输入绑定20250819.vue'
  import props from './components/props20250819.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // if20250818
    // forms
    // process
    // model
    props
  },
  data(){
    return{
    message:"hello",
    age:30,
    name:["hoshino", "tsukino"],
    }
  }
}
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
