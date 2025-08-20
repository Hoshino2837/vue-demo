<template>
    <h1>20250818条件渲染</h1>
    <div v-if="flag">公孙离</div>
    <div v-else="flag">张良</div>
    <div v-show="flag">hoshino</div>
</template>
<script>
    export default{
        name:"if",
        data(){
            return{
            flag:true
            }
        }
    }
</script>