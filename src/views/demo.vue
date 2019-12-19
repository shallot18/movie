<template>
    <!--template代表的就是HTML的内容，相当于<div id="app">标签中的内容-->
    <!--//必须要有根节点-->
    <div>
        <h1>{{content}}</h1>
        请输入内容:<input type="text"v-model="content">
        <el-button type="warning"round>一个按钮</el-button>
    </div>
</template>
<script>
    import ElButton from "../../node_modules/element-ui/packages/button/src/button";
    export default{
        //在.vue文件中定义data必须使用function,原因是每一个页面都保存了自己的数据
        components: {ElButton},
        data:function () {
            //return返回数据，将对象通过return返回vue-cli
            return{
                content:""  //定义了一个content
            }
        }
    }
</script>
<!--scooed含义：将当前vue文件中css属性的作用域限制在当前的页面，不会对其他页面产生影响-->
<style scoped>
    h1{
        color: red;
    }
</style>