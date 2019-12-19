<template>
<div>
    <div class="wrapper">
        <div class="content">
           <h2 >豆瓣电影排行榜</h2>
            <div class="artical">
                <p1 style="color: #007722" >豆瓣新片榜......</p1>
                <div class="indent">
                    <p class="dashed"></p>

              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2568902055.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/6981153/">
                          {{movie_1.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_1.releaseDate}}
                       {{movie_1.pointProjection}}
                       {{movie_1.netWork}}
                       {{movie_1.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_1.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_1.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_1.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>
    </div>
                <div class="indent2">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2567198874.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/27119724/">
                          {{movie_2.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_2.releaseDate}}
                       {{movie_2.netWork}}
                       {{movie_2.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_2.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_2.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_2.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>
    </div>
                <div class="indent3">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2570137991.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/30327842/">
                          {{movie_3.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_3.releaseDate}}
                       {{movie_3.netWork}}
                       {{movie_3.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_3.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_3.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_3.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>

    </div>
                <div class="indent4">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2551119672.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2551119672.webp">
                          {{movie_4.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_4.releaseDate}}
                       {{movie_4.pointProjection}}
                       {{movie_4.netWork}}
                       {{movie_4.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_1.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_4.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_4.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>
    </div>
                <div class="indent5">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2571760178.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/27202818/">
                          {{movie_5.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_5.releaseDate}}
                       {{movie_5.pointProjection}}
                       {{movie_5.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_5.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_5.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_5.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>
    </div>
                <div class="indent6">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2561370606.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/27594938/">
                          {{movie_6.name}}
                      </a>
                      </div>
                     <div class="content">
                       {{movie_6.releaseDate}}
                       {{movie_6.cast}}
                     </div>
                      <div class="xing_1">
                          <el-rate disabled v-model="movie_6.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_6.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_6.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>
    </div>
                <div class="indent7">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2570825762.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/26858510/">
                          {{movie_7.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_7.releaseDate}}
                       {{movie_7.pointProjection}}
                       {{movie_7.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_7.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_7.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_7.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>
    </div>
                <div class="indent8">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2564884269.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/10546436/">
                          {{movie_8.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_8.releaseDate}}
                       {{movie_8.pointProjection}}
                       {{movie_8.netWork}}
                       {{movie_8.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_8.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_8.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_8.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>
    </div>
                <div class="indent9">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2549891899.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/30241102/">
                          {{movie_9.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_9.releaseDate}}
                       {{movie_9.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_9.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_9.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_9.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>

    </div>
                <div class="indent10">
                    <p class="line1"></p>
              <el-row type="flex" justify="center">
                 <el-col :span="4"class="indent_1">
                  <img  src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2556824333.webp"/>
                 </el-col>
                  <el-col :span="24">
                      <div class="title_1">
                      <a href="https://movie.douban.com/subject/27089612/">
                          {{movie_10.name}}
                      </a>
                      </div>
                     <div class="content_1">
                       {{movie_10.releaseDate}}
                       {{movie_10.cast}}
                     </div>
                      <div class="xing">
                          <el-rate disabled v-model="movie_10.scoring.star" style="display: inline-block"></el-rate>
                          <div class="fenshu">
                              {{movie_10.scoring.score}}
                              <span style="font-size: 13px;color: #616266; float: right;line-height: 22px;">
                              ({{movie_10.comment.people}})人评价
                              </span>
                          </div>
                      </div>
                  </el-col>
              </el-row>

    </div>
    </div>
    </div>
    </div>
</div>
</template>
<script>
    import ElRate from "../../node_modules/element-ui/packages/rate/src/main";
    import ElCol from "element-ui/packages/col/src/col";
    import ElProgress from "../../node_modules/element-ui/packages/progress/src/progress";
    import ElButton from "../../node_modules/element-ui/packages/button/src/button";
    import ElRow from "element-ui/packages/row/src/row";
    export default{
        components: {
            ElRow,
            ElButton,
            ElProgress,
            ElCol,
            ElRate},
        data(){
            return{
                movie_1:{
                    name:'爱尔兰人 / 爱尔兰杀手(港) / 听说你刷房子了',
                    releaseDate:'2019-09-27(纽约电影节)',
                    pointProjection:'2019-11-01(美国点映) ',
                    netWork:'2019-11-27(美国网络)',
                    cast:'/罗伯特·德尼罗/'+  '/阿尔·帕西诺/ ' +
                    ' 乔·佩西 / 安娜·帕奎因 / 杰西·普莱蒙 / ' +
                    '哈威·凯特尔 / 斯蒂芬·格拉汉姆 / 鲍比·坎纳瓦尔 /' +
                    ' 杰克·休斯顿 / 阿莱卡萨·帕拉迪诺 / 凯瑟琳·纳杜奇...',
                    scoring:{
                        star:4.5,
                        score:9.1,
                    },
                    comment:{
                        people:46812
                    }
                },
                movie_2:{
                    name:'丑起源电影：罗密欧 / Romeo',
                    releaseDate:'2019-08-31(威尼斯电影节)',
                    pointProjection:'2019-10-04(美国点映) ',
                    netWork:'2019-11-27(美国网络)',
                    cast:'/ 杰昆·菲尼克斯/'+  '/罗伯特·德尼罗/ ' +
                    ' 马克·马龙 / 莎姬·贝兹  / 谢伊·惠格姆/ ' +
                    '弗兰西丝·康罗伊 / 布莱恩·考伦/ 布莱恩·泰里·亨利 /' +
                    ' 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒...',
                    scoring:{
                        star:4.5,
                        score:8.8,
                    },
                    comment:{
                        people:379637
                    }
                },
                movie_3:{
                    name:'英 / 82年生金智英 / Kim Ji-young,Born 1982',
                    releaseDate:'2019-10-23(韩国)',
                    pointProjection:'2019-11-07(中国香港) ',
                    cast:'/ 郑有美/'+  '/孔侑/ ' +
                    ' 金美京 / 孔敏晶 / 朴成妍 / ' +
                    '李凤莲 / 金圣喆 / 李乌 /' +
                    ' 李海云 /  孙成灿 / 金正英...',
                    scoring:{
                        star:4.5,
                        score:8.7,
                    },
                    comment:{
                        people:37143
                    }
                },
                movie_4:{
                    name:'从前，有个荷里活(港) / 从前，有个好莱坞...(台)',
                    releaseDate:'2019-05-21(戛纳电影节)',
                    pointProjection:'2019-07-26(美国) ',
                    netWork:'2019(中国大陆)',
                    cast:'/莱昂纳多·迪卡普里奥/'+  '/布拉德·皮特 / ' +
                    ' 玛格特·罗比  /  埃米尔·赫斯基 /玛格丽特·库里 / ' +
                    '蒂莫西·奥利芬特 / 茱莉亚·巴特斯 / 奥斯汀·巴特勒 /' +
                    ' 达科塔·范宁 / 布鲁斯·邓恩 ...',
                    scoring:{
                        star:3.5,
                        score:7.3,
                    },
                    comment:{
                        people:73954
                    }
                },
                movie_5:{
                    name:'婚姻故事',
                    releaseDate:'2019-08-29(威尼斯电影节)',
                    pointProjection:'2019-12-06(美国) ',
                    cast:'/斯嘉丽·约翰逊/'+  '/亚当·德赖弗/ ' +
                    ' 梅里特·韦弗 / 劳拉·邓恩 / 雷·利奥塔 /  ' +
                    '朱丽·哈基提 / 马克·奥布莱恩 / 华莱士·肖恩 / ' +
                    '  阿伦·阿尔达 / 凯尔·柏海莫 / 米奇·萨姆纳...',
                    scoring:{
                        star:4.5,
                        score:8.8,
                    },
                    comment:{
                        people:21367
                    }
                },
                movie_6:{
                    name:'准备好了没 / 弑婚游戏(台) / 爆血新婚夜(港)',
                    releaseDate:'2019-08-21(美国)',
                    cast:'/ 萨玛拉·维文/'+  '/安迪·麦克道威尔/ ' +
                    ' 马克·奥布莱恩 / 亚当·布罗迪 / 亨利·科泽尼 / ' +
                    '妮基·瓜达尼 / 梅兰妮·斯科洛凡诺 / 克里斯蒂安·布鲁恩 /' +
                    ' 伊利斯 莱韦斯克 / 约翰·拉尔斯顿...',
                    scoring:{
                        star:3.5,
                        score:6.7,
                    },
                    comment:{
                        people:26430
                    }
                },
                movie_7:{
                    name:'克劳斯：圣诞节的秘密 / 圣诞老人',
                    releaseDate:'2019-11-08(西班牙))',
                    pointProjection:'2019-11-08(英国)  ',
                    cast:'/J·K·西蒙斯/'+  '詹森·舒瓦兹曼/ ' +
                    ' 拉什达·琼斯 / 琼·库萨克 / 诺曼·麦克唐纳徳 /  ' +
                    '威尔·萨索 / 塞尔希奥·巴勃罗斯 / 米拉·布雷纳 /' +
                    ' 内达·玛格丽特·拉巴 / 悉尼·布朗 / 泰迪·布鲁姆...',
                    scoring:{
                        star:4.5,
                        score:8.6,
                    },
                    comment:{
                        people:7743
                    }
                },
                movie_8:{
                    name:'第一滴血5：最后的血 / 第一滴血：终极血战(港) / 蓝波：最后一滴血(台)',
                    releaseDate:'2019-09-18(印度尼西亚)',
                    pointProjection:' 2019-09-20(美国) ',
                    netWork:'2019-09-27(西班牙)',
                    cast:'/西尔维斯特·史泰龙/'+  '/帕斯·贝加/ ' +
                    ' 塞尔吉奥·佩里斯-门切塔 / 艾德里安娜·巴拉扎 / 维特·蒙雷尔 / ' +
                    '吉妮·金 / 华金·科西奥 / 帕斯卡西奥·洛佩斯 /' +
                    ' 奥斯卡·贾恩那达 / 亚历山大·迪米特罗夫...',
                    scoring:{
                        star:4,
                        score:7.5,
                    },
                    comment:{
                        people:14782
                    }
                },
                movie_9:{
                    name:'行骗天下JP：浪漫篇 / 信用欺诈师JP:香港浪漫篇(港) / 行骗天下 电影版',
                    releaseDate:'2019-05-17(日本) ',
                    cast:'/长泽雅美/'+  '/东出昌大/ ' +
                    '  小日向文世 / 竹内结子 / 三浦春马 / ' +
                    '江口洋介 / 小手伸也 / 织田梨沙 /' +
                    '  前田敦子 / 小栗旬 / 佐津川爱美...',
                    scoring:{
                        star:4,
                        score:8.3,
                    },
                    comment:{
                        people:9061
                    }
                },
                movie_10:{
                    name:'纽约的一个雨天 / 情迷纽约下雨天(港) / 纽约有雨',
                    releaseDate:'2019-07-26(波兰)',
                    cast:'/蒂莫西·柴勒梅德/'+  '/艾丽·范宁/ ' +
                    ' 赛琳娜·戈麦斯 / 裘德·洛 / 迭戈·卢纳 / ' +
                    '列维·施瑞博尔 / 苏琪·沃特豪斯 / 凯莉·罗尔巴赫 /' +
                    ' 丽贝卡·豪尔 / 安娜莱吉·阿什福特 / 切莉·琼斯...',
                    scoring:{
                        star:4,
                        score:7.5,
                    },
                    comment:{
                        people:5624
                    }
                },
            }
        }
    }
</script>
<style scoped>
   .wrapper{
       width: 1200px;
       margin: 0 auto;
   }
   .content h2{
       padding-right: 850px;
       color:#494949;
       font-size: 26px;
   }
    p{
        border-bottom: 1px dashed #dddbd8;
    }
   .indent_1 img{

       width:  110px;
   }
   .title_1{
       text-align: left;
       margin-bottom: 5px;
   }
   .content{
       text-align: left;
   }
    .xing{
        text-align: left;
        font-size: 12px;
        color: #e09015;
        display: inline-block;
        float: left;
    }
    .fenshu{
        float: right;
        line-height: 22px;
    }
</style>