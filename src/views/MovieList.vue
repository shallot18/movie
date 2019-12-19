<template>
    <div>
        <el-row style="margin-top: 10px">
            <el-col :span="4">
                <el-radio label="按热度排序"></el-radio>
            </el-col>
            <el-col :span="4">
                <el-radio label="按时间排序"></el-radio>
            </el-col>
        </el-row>
        <hr/>
        <el-row v-for="subList in movieList" type="flex" justify="center"
        style="margin-top: 20px">
               <el-col :span="4">
                   <img v-bind:src="subList[0].imgUrl"/>
                   <div>
                       <span class="title-span"v-on:click="detailPage(subList[0].title)">{{subList[0].title}}</span>
                       &nbsp;&nbsp;
                       <span class="scroe-span">{{subList[0].score}}</span>
                   </div>
               </el-col>

               <el-col :span="4">
                   <img v-bind:src="subList[1].imgUrl"/>
                   <div>
                       <span class="title-span"v-on:click="detailPage(subList[1].title)">{{subList[1].title}}</span>
                       &nbsp;&nbsp;
                       <span class="scroe-span">{{subList[1].score}}</span>
                   </div>
               </el-col>

               <el-col :span="4">
                   <img v-bind:src="subList[2].imgUrl"/>
                   <div>
                       <span class="title-span"v-on:click="detailPage(subList[2].title)">{{subList[2].title}}</span>
                       &nbsp;&nbsp;
                       <span class="scroe-span">{{subList[2].score}}</span>
                   </div>
               </el-col>

               <el-col :span="4">
                   <img v-bind:src="subList[3].imgUrl"/>
                   <div>
                       <span class="title-span"v-on:click="detailPage(subList[3].title)">{{subList[3].title}}</span>
                       &nbsp;&nbsp;
                       <span class="scroe-span">{{subList[3].score}}</span>
                   </div>
               </el-col>

               <el-col :span="4">
                   <img v-bind:src="subList[4].imgUrl"/>
                   <div>
                       <span class="title-span"v-on:click="detailPage(subList[4].title)">{{subList[4].title}}</span>
                       &nbsp;&nbsp;
                       <span class="scroe-span">{{subList[4].score}}</span>
                   </div>
               </el-col>
        </el-row>
    </div>
</template>
<script>
    export default{
        data: function () {
            return {
                movieList: [
                    [
                        {title:'小丑',score:8.4,imgUrl:require('../assets/1.jpg')},
                        {title:'好莱坞往事',score:7.4,imgUrl:require('../assets/2.jpg')},
                        {title:'非凡夏日',score:7.5,imgUrl:require('../assets/3.jpg')},
                        {title:'我在你床下',score:6.7,imgUrl:require('../assets/5.jpg')},
                        {title:'酷刑报告',score:7.0,imgUrl:require('../assets/6.jpg')}
                    ],
                    [
                        {title:'爱尔兰人',score:9.1,imgUrl:require('../assets/6.jpg')},
                        {title:'攀登者',score:6.2,imgUrl:require('../assets/7.jpg')},
                        {title:'准备好了没',score:6.8,imgUrl:require('../assets/8.jpg')},
                        {title:'双子杀手',score:7.1,imgUrl:require('../assets/9.jpg')},
                        {title:'地久天长',score:8.0,imgUrl:require('../assets/10.jpg')}
                    ]
                ]
            }
        },
        methods:{
            detailPage:function(title){
                /**
                 * 获取router对象，调用router对象的push方法
                 * this 因为是movieList调用
                 * router是编程式跳转页面
                 * <router-link to="/demo">Demo</router-link>则是声明式跳转页面
                 */
                this.$router.push({name:"movie",params:{title:title}});
            }
        }
    }
</script>
<!--ctrl+alt+l 快速格式代码-->
<!--scoped用于编写div样式-->
<style scoped>
     img{
         width:160px;
         height:240px;
     }
    .title-span{
        cursor: pointer;
        color:#37a ;
    }
    .scroe-span{
        color:#e09015;
    }
</style>