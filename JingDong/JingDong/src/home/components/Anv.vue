<!--  -->
<template>
<div class='anv'>
    <div class="wrapper">
         
            
         <div class="flex-box">
            <ul> 
                  
                <li class="lx"><span class="iconfont">&#xe61b;</span>
                广东</li>
               
               
                <li>你好，请登录  免费注册</li>
                <li>我的订单</li>
                <li>我的京东
                    <span class="iconfont bottom-icon">&#xe658;</span>
                </li>
                <li>京东会员</li>
                <li class="jk">企业采购
                    <span class="iconfont bottom-icon">&#xe658;</span>
                </li>
                <li>客户服务
                   <span class="iconfont bottom-icon">&#xe658;</span>
                </li>
                <li>网站导航
                    <span class="iconfont bottom-icon">&#xe658;</span>
                </li>
                <li>手机京东</li>
               
                
            </ul>
         
         </div>
        
    </div>

  
</div>
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';
//import Swiper from "swiper";

export default {
name:'HomeAnv',
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
.anv
    overflow: hidden
    height: 0
    padding-bottom: 1.6%
    background: #e3e4e5
    .wrapper
        lign-height: 31px
       
        position: relative
        .flex-box
           
            width: 1190px
            height: 31px
            line-height:31px
            margin: 0 356.5px
            text-align: center
            position: absolute
           
            
           
            
            
            
            ul
              
               
               display: flex
               font-size: 12px
               align-height: 31px
               
               flex-wrap: nowrap
               justify-content: space-between
               color: 999  
               overflow:hidden
               white-space:nowrap
               text-overflow:ellipsis  
               .jk
                  color: #f10215
               .lx
                  padding-right: 440px
                  
                 
                  
                  
                 
                     

     
        
       
                 

            
            
                
            
            
            

           

</style>