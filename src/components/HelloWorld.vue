<template>
  <div class="hello">
    <h1>vue学习</h1>
    <h2>{{ msg }}</h2>
    <h3>{{ massage }}</h3><!-- {{  }} 中是动态文本，可变-->
    <div>{{ HTML }}</div> <!--通过文本形式展示-->
    <div v-html="HTML"></div> <!--通过网页语句形式展示-->
    <div :id="Hid"></div><!--设置id-->
    <div>{{ person>10 ? "很多":"很少" }}</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      massage:"星野vue", 
      msg: "today is 20250818 Monday",
      HTML: "<a href='https://www.baidu.com'>百度一下</a>",//创建一个a标签
      Hid:"cat",
      person:10
    }
  }
}
</script>

