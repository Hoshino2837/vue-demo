<template>
    <h2>自定义组件交互20250820</h2>
    <h3>hohsino</h3>
    <button @click="trans">传递数据</button>
</template>
<script>
    export default{
        name:"emit",
        data(){
            return{
                message:"数据传递成功！"
            }
        },
        methods:{
            trans(transContent){
                //俩参数，第一个是名称，第二个是参数
                this.$emit("transfer",this.message);
            }
        }
    }
</script>
<style scoped>
</style>