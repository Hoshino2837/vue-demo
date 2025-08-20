<template>
    <h2>生命周期(life cycle)</h2>
    <p>{{ message }}</p>
    <button @click="count+=1">{{ count }}</button>
</template>
<script>
    export default{
        data(){
            return{
                message:"start",
                count:0
            }
        },
        beforeCreate(){
            console.log("beforeCreate:组件创建之前")
        },
        created(){
            console.log("create:创建之时")
        },
        beforeMount(){
            console.log("beforeMount:挂载之前")
        },
        mounted(){
            console.log("mounted:挂载之时");
        },
        beforeUpdate(){
            console.log("beforeUpdate:更新之前");
        },
        updated(){
            console.log("updated:更新之时");
        },
        beforeUnmount(){
            console.log("beforeUnmount:卸载之前");
        },
        unmounted(){
            console.log("unmount:卸载之时");
        }
    }
</script>