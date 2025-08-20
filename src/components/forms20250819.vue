<template>
    <ul>
    <li :id="form" v-for="(item,) in items" :key="item.id">{{ item.message }}</li>
    </ul>
</template>
<script>
    export default{
        name:"forms",
        data(){
            return{
                items:[{
                    id:1,
                    message:"hoshino"},
                    {
                    id:2,    
                    message:"星野"}]
            }
        }
    }
</script>