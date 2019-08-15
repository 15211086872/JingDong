<!--  -->
<template>
<div class='top border-bottom'>
    <div class="w">
        <div class="logo">
            <img class="logo-image" src="http://www.szquanli.com/uploads/allimg/170831/2-1FS1095324-52.png" 
            />         
         </div> 
 
        <div class="searh-m">
            <div class="form">
              
                <input  class="search" type="text" placeholder="投影仪家用" /></div>
            <div class="iconfont camera-icon">
                &#xe62a;                                        
            </div>
            <div class="cw-icon">
               <i class="iconfont">&#xe62c;</i>
               我的购物车
               
            </div>
        </div>
        <div class="hotwords">
           <ul>
               <li id="imp">精品百货节</li>
               <li>空调钜惠</li>
               <li>缤纷水饮</li>
               <li>个护神券</li>
               <li>每100-50</li>
               <li>面膜</li>
               <li>二手浪琴</li>
               <li>家装建材</li>
               <li>199减100</li>
           </ul>
         <div class="spacer">
           <ul>
               <li id="uzi">秒杀</li>
               <li id="shy">优惠券</li>
               <li>PLUS会员</li>
               <li>品牌闪购</li>
               <li>拍卖</li>
               <li>京东时尚</li>
               <li>京东超市</li>
               <li>京东生鲜</li>
               <li>海囤全球</li>
               <li>京东金融</li>
           </ul>
         </div>  
           
         </div>
         <div class="J_mobile_pop">
            <img class="cute" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1565612095381&di=7c7568bdba97f11d6a0c015b84e04a34&imgtype=0&src=http%3A%2F%2Fmmbiz.qpic.cn%2Fmmbiz_png%2F5DLkyBhaHiazcibPeasn6kjiaOoNyuicaBvHp7ncdn4sE0NOYsicg37jIDRH1ykN1sww5sB4gDBh5cfdBlDS51r7Yug%2F640%3Fwx_fmt%3Dpng"/>
         </div>
    </div>
 
</div>
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';
//import Swiper from "swiper";

export default {
name:'HomeTop',
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
//这里存放数据
return {

};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合 专门存放方法比如点击事件
methods: {

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
.top
   overflow: hidden
   width: 100%
   height: 0
   padding-bottom: 7.4%
   background: fff

   .w
      width: 990px
      height: 140px
      margin: 0 210px
      color: 666
      .logo
         position: absolute
         width: 190px
         height: 120px
         float: left 
         .logo-image
            width: 100%
            height: 120px
            padding-top: 10px
      .searh-m
         overflow: hidden
         position: absolute
         width: 990px
         height: 64px
         float: left
         
         .form
           
            position: relative
            float: left
            margin-left: 260px
            margin-top: 24px 
            width: 490px
            height: 36px
            border: 2px solid red
            .search
              
               
               
              
               width: 430px
               height: 32px
               padding: 2px 44px 2px 17px
        
            
         .camera-icon
            font-size: 20px
            margin-left: 754px
            margin-top: 24px
            position: absolute
            float: left 
            background: red
            text-align: center
            line-height: 40px
            width: 58px
            
            
         .cw-icon
            float: left 
            border: 1px solid #666666
            color: #e1251b
            width: 132px
            height: 36px
            line-height: 36px
            margin-top: 24px
            margin-left:78px
            text-align:center
      .hotwords
        
         position: absolute
         float: left
         width: 550px
         height: 20px
         margin-left: 260px
         margin-top: 69px
         ul
            display: flex
            justify-content: space-between
            flex-wrap: nowrap
            color: #999
            font-size: 12px
            #imp
               color: #e1251b 
      .spacer
         position: absolute 
         float:left
         width: 761.72px
         height:40px
         line-height: 40px
         margin-top: 20px
         margin-left: -50px
         ul
            color: #333333
            font-size: 15px
            #uzi,#shy
               color: #e1251b
               font-weight: bold
      .J_mobile_pop
         position: absolute
         width: 76px
         height: 76px
         float: left
         margin-left: 1270px
         margin-top: 10px
         .cute
            width: 100%
            height: 66px
            line-height:66px
            
         
               
            
         
            
               
           
               
                 



            
            
              
         
 
</style>