<template>
    <input v-model="username" placeholder="请输入user"></input>
    <div>{{ username }}</div>
    <!--加上trim来去除空格-->
    <input v-model.trim="password" placeholder="请输入password"></input>
    <div>{{ password }}</div>
    <button @click="userNameGet">获取用户名</button>
</template>
<script>
    export default{
        data(){
            return{
                username:null,
                password:null
            }
        },
        methods:{
            userNameGet(){
                console.log(this.username);
                console.log(this.password);
            }
        }
    }
</script>