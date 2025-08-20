<template>
    <div>{{ count }}</div>
    <button @click="count += 1">+1</button>
    <button @click="method">reset</button>
    <div @mousemove="count += 1" :id="move">move</div>
    <div :id="uls">
        <ul>
            <li @click="clickName(name)" v-for="(name, index) in names" :key="index">{{ name }}</li>
        </ul>
    </div>
</template>
<script>
export default {
    data() {
        return {
            uls: "uls",
            count: 1,
            move: "move",
            myform: "myform",
            names: ["hoshino", "tsukino", "tiga"]
        }
    },
    methods: {//事件处理方法
        method() {
            this.count = 0;
            alert("count已被重置")
        },
        clickName(name) {
            console.log(name);
            alert("点击了"+name);
        }
    }
}
</script>
<style scoped>
#move {
    position: absolute;
    left: 260px;
    top: 100px;
    width: 200px;
    height: 200px;
    background-color: #ffc0cb;
}
#uls {
    width: 50px
}
</style>