<template>
    <h1>{{ message }}</h1>
    <div v-for="(names,index) in name":key="index">{{ names }}</div>
    <div>{{ age }}</div>
</template>
<script>
export default{
    name:"props",
    props:{
        message:{
        type:String,
        default:""
    },
        name:{
      type:Array,
      default:()=> {
        [ ]
      }
    },
     age:{
        type:Number,
        default:null
      }
    }
    }
</script>