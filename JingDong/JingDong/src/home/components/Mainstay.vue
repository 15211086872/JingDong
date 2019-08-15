<!--  -->
<template>
<div class='mainstay'>
    <div class="room">
        <div class="J_cate">
            <ul>
                <li>家用电器</li>
                <li>手机 / 运营商 / 数码</li>
                <li>电脑 / 办公</li>
                <li>家居 / 家具 / 家装 / 厨具</li>
                <li>男装 / 女装 / 童装 / 内衣</li>
                <li>美妆 / 个护清洁 / 宠物</li>
                <li>女鞋 / 箱包 / 钟表 / 珠宝</li>
                <li>男鞋 / 运动 / 户外</li>
                <li>房产 / 汽车 / 汽车用品</li>
                <li>母婴 / 玩具乐器</li>
                <li>食品 / 酒类 / 生鲜 / 特产</li>
                <li>艺术 / 礼品鲜花 / 农资绿植</li>
                <li>医药保健 / 计生情趣</li>
                <li>图书 / 文娱 / 电子书</li>
                <li>机票 / 酒店 / 旅游 / 生活</li>
                <li>理财 / 众筹 / 白条 / 保险</li>
                <li>安装 / 维修 / 清洗 / 二手</li>
                <li>工业品</li>
            </ul>
        </div>
        <div class="wrapper">
                <swiper :options="swiperOption" v-if="showSwiper">
            
                <swiper-slide v-for="item of list" :key="item.id">
                    <img class="swiper-img" :src="item.imgUrl"/>
                </swiper-slide>
                
                <div class="swiper-pagination"  slot="pagination"></div>
                <div class="swiper-button-prev" slot="button-prev"></div>
                <div class="swiper-button-next" slot="button-next"></div>
            
            </swiper>
        </div>
        <div class="content">
            <img class="otto" src="//img30.360buyimg.com/babel/s380x300_jfs/t1/81165/22/6039/93080/5d43a5e6Ed88426de/5b0d0d349d369343.jpg.webp"/>
            <img class="rookie" src="//img13.360buyimg.com/babel/s380x300_jfs/t1/84506/9/6647/86095/5d4a7fc2E7357b5b8/d2a537d26b630502.png.webp"/>
            <img class="iboy" src="//img14.360buyimg.com/babel/s380x300_jfs/t1/61180/22/7004/85128/5d50cdfdE765adaa3/f64e6c21ffb78de3.jpg.webp"/>

        </div>
        <div class="right">
            <div class="first border-bottom" >
               <div class="me">
                  <div class="xiaogou">
                      <img src="data:image/png;base64,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"/>
                  </div>
                  <div class="xiaohu">
                       <p class="zoom">Hi~欢迎逛京东！</p>
                       <p>登录 | 注册</p>
                  </div>
               </div>
               <div class="him">
                   <div class="tim">
                       新人福利

                   </div>
                   <div class="tom">
                        PLUS会员
                   </div>
                      
               </div>

               
            </div>
            <div class="second border-bottom">
                <div class="ig">
                    <span class="pap">京东快报</span>
                    <span class="pop">更多></span>
                </div>
                <ul>
                    <li>
                        <div class="zu">
                            <span class="huang">推荐</span>
                            华为鸿蒙系统，操作方式类似iOS 13，花粉们都尖叫了
                        </div>
                    </li>
                    <li>
                        <div class="zu">
                            <span class="huang">热门</span>
                            iPhoneSE2概念图：屏下指纹识别 
                        </div>
                    </li>
                    <li>
                        <div class="zu">
                            <span class="huang">最新</span>
                            华为有新动作！麒麟980+8GB+性价比，用户不淡定了
                        </div>
                    </li>
                    <li>
                        <div class="zu">
                            <span class="huang">热议</span>
                            米粉乐了！续航120公里的小米电动车上市！价格便宜！
                        </div>
                    </li>
                </ul>

            </div>
            <div class="third border-bottom">
                <ul>
                    <li v-for="item of smallList" :key="item.id">
                        <img :src="item.imgUrl"/>
                        <p>{{item.desc}}</p>
                    </li>
                </ul>

            </div>

        </div>
    </div>
</div>
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';
//import Swiper from "swiper";

export default {
name:'HomeMainstay',
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
  
//这里存放数据
return {
    list: [
    {
        id: '0001',
        imgUrl: "//img12.360buyimg.com/babel/s590x470_jfs/t1/79864/28/6899/95579/5d4c1dacE4eb9b16d/5e895c796e7ff9ab.jpg.webp"
    },
    {
        id: '0002',
        imgUrl: "//img14.360buyimg.com/pop/s590x470_jfs/t1/72532/2/6659/100249/5d4ce7c0Ecafd257c/ccb76ff80d343b55.jpg.webp"
    },
    {
        id: '0003',
        imgUrl: "//img20.360buyimg.com/pop/s590x470_jfs/t1/64351/28/6672/56158/5d4abe9dEd77ced8b/f80b214d81779fdb.jpg.webp"
    },
    {
        id: '0004',
        imgUrl: "//imgcps.jd.com/ling/23275739740/5YW76L2m5bCP6L6-5Lq6/5aW954mp5L2O6IezOS455YWD5ou8/p-5bd8253082acdd181d02f9ee/7616ede7.jpg"
    },
    {
        id: '0005',
        imgUrl: "//img30.360buyimg.com/pop/s590x470_jfs/t1/58681/28/6146/128428/5d43f72dEf3895cc5/0662870d44220491.jpg.webp"
    },
    {
        id: '0006',
        imgUrl: "//imgcps.jd.com/ling/53346196849/6Iqx5aW95pyI5ZyG/5ruhMTk55YePMzA/p-5bd8253082acdd181d02fa6d/71cae52f.jpg"
    },
    {
        id: '0007',
        imgUrl: "//img12.360buyimg.com/pop/s590x470_jfs/t1/76447/18/6631/72607/5d4d41c6E80f53918/f47d2dd2826bb2c4.png.webp"
    },
    

    ],
    smallList: [
       {
        id: '0001',
        imgUrl: "//m.360buyimg.com/babel/jfs/t1/30057/19/14881/720/5cbf064aE187b8361/eed6f6cbf1de3aaa.png",
        desc: '话费'
    },
    {
        id: '0002',
        imgUrl: "//m.360buyimg.com/babel/jfs/t1/36478/38/5384/2901/5cbf065aEb0c60a12/afb4399323fe3b76.png",
        desc: '机票'
    },
    {
        id: '0003',
        imgUrl: "//m.360buyimg.com/babel/jfs/t1/31069/34/14642/979/5cbf0665Ec7dc8223/5fee386254dd2ebc.png",
        desc: '酒店'
    },
    {
        id: '0004',
        imgUrl: "//m.360buyimg.com/babel/jfs/t1/32403/22/14829/3699/5cbf0674E04723693/caa83ce9b881cd24.png",
        desc: '游戏'
    },
    {
        id: '0005',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/39418/35/2029/3048/5cbf06bbE9a6e2beb/6a9b204b0a4cc3d0.png",
        desc: '加油卡'
    },
    {
        id: '0006',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/31847/11/14820/1581/5cbf09bdE07a1e79c/1281c9340ef15c3e.png",
        desc: '火车票'
    },
    {
        id: '0007',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/33078/37/6694/1685/5cbf09d0E5cea6165/693857001bfb3b17.png",
        desc: '众筹'
    },
    {
        id: '0008',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/35979/1/3099/3447/5cbf09e4E90c0b4f4/e632d50688935da6.png",
        desc: '理财'
    },
    {
        id: '0009',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/35663/12/5436/1443/5cbf0a13E614f5bb0/6ab7c7eb7caa4656.png",
        desc: '白条'
    },
    {
        id: '0010',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/34018/19/6744/3066/5cbf09a9Eef05e8bd/6a08fe38fa0f8143.png",
        desc: '电影票'
    },
    {
        id: '0011',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/74010/31/656/1821/5cedfd1dE574a6d39/21ed5b49bcde9067.png",
        desc: '企业购'
    },
    {
        id: '0012',
        imgUrl: "http://m.360buyimg.com/babel/jfs/t1/35852/40/5378/815/5cbf09f9E660e7e71/18b5679ed16e6a91.png",
        desc: '礼品卡'
    },
  
    ],
    swiperOption: {
         pagination: ".swiper-pagination",
         paginationClickable: true,
         prevButton: ".swiper-button-prev",
         nextButton: ".swiper-button-next",
         autoplay: 1000,
         loop: true


    }
    

};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合 专门存放方法比如点击事件
methods: {
    showSwiper (){
        return this.list.length
    }

},
//生命周期 - 创建完成（可以访问当前this实例）
created() {

},
//生命周期 - 挂载完成（可以访问DOM元素）
mounted() {
//this.getData();//加载完后执行getData这个函数

},
beforeCreate() {}, //生命周期 - 创建之前
beforeMount() {}, //生命周期 - 挂载之前
beforeUpdate() {}, //生命周期 - 更新之前
updated() {}, //生命周期 - 更新之后
beforeDestroy() {}, //生命周期 - 销毁之前
destroyed() {}, //生命周期 - 销毁完成
activated() {}, //如果页面有keep-alive缓存功能，这个函数会触发
}
</script>
<style lang="stylus" scoped>
.mainstay
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 25.2%
    color: #666666
    background: #f4f4f4
    .room
        
        margin: 0 356.5px

        .J_cate
            width: 190px
            padding-bottom: 100%
            line-height: 100%
            float: left 
            background: #fefefe
            margin-top: 10px
           
            ul
              
               font-size: 14px
               color: #333
               padding: 10px 0px 0 18px
               li
                  padding-bottom: 11.5px
        .wrapper >>> .swiper-pagination-bullet-active
           background: #fff
        .wrapper >>> .swiper-button-prev 
           color: #ffffff
           width: 20px
           height: 20px
           background-size: 25px 30px
        .wrapper >>> .swiper-button-next 
           color: #ffffff
           width: 20px
           height: 20px
           background-size: 25px 30px          
        .wrapper
           margin: 10px 0px 0px 10px
           width: 590px
           padding-bottom: 100%
           float: left
           .swiper-img
              width: 100%
        .content
           
           margin: 10px 0px 0px 10px
           width: 190px
           padding-height: 100%
           float: left
           
           img
              width: 100%
              padding-bottom: 10px
        .right
           padding: 10px 0px 0px 10px
           width: 190px
           padding-bottom: 100%
           float: left
           
           .first
              overflow: hidden
              width: 100%
              height: 102px
              background: #ffffff
             
                 
              .xiaogou
                 width: 40px
                 height: 0 
                 margin: 20px 0px 0px 20px
                 
                 img 
                    width: 100%
               .xiaohu
                  color: #333
                  float: left
                  margin-left: 70px
                  width: 106px
                  height: 38px
                  p
                     padding-bottom: 10px
                     
                  .zoom
                     color: #666
           .tim
              width: 70px
              height: 25px
              line-height: 25px
              color: #ffffff
              background: #e1251b
              float: left
              margin-top: 10px
              margin-left: 20px
              text-align: center
              border-radius: 15px
            .tom
              width: 70px
              height: 25px
              line-height: 25px
              color: #e5d790
              background: #363634
              float: left
              margin-top: 10px
              margin-left: 10px
              text-align: center
              border-radius: 15px
        .second
           overflow: hidden
           width: 100%
           height: 130px
           background: #fff
           .ig
              width: 190px
              height: 3opx
              margin: 0 0 8px 
              padding: 10px
              span 
                 padding-right: 70px
              .pap
                 font-size: 14px
                 font-weight: bold
                 color: #333
              .pop
                 font-size: 12px
                 color: #999
           ul
              float: left
              margin-left: 10px
              .zu
                 height: 16px
                 line-height: 16px
                 font-size: 12px
                 overflow: hidden
                 white-space: nowrap
                 text-overflow: ellipsis
                 max-width: 160px
                 padding-bottom: 6px
                .huang
                    color: #e1251b
                    background:rgba(225,37,27,0.08)
        .third{
            width: 100%
            overflow: hidden
            background: #fff
            ul{ 
                display: flex
                justify-content: space-around
                flex-wrap: wrap
                text-align: center

                li{
                    padding: 6px 0
                    width: 33.3%
                    img{
                        width: 44.5%
                        padding-bottom: 5px
                    }
                }
            }
        }
            

                 
                 
                   

              
             
              
                

                        
                    
              
          



                  

            
                
        

        

</style>