<!--  -->
<template>
<div class='header' v-show= "visible">
    <div class="img-top">
        <button class= "delete" @click= "show" >x</button>
        <img class="header-image"
        src="//img20.360buyimg.com/da/jfs/t1/48708/29/7147/49138/5d4b92deE3d9c411b/8852243f22ad3ac8.jpg.webp"
        />
       
    </div>
 
</div>
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';
//import Swiper from "swiper";

export default {
name:'HomeHeader',
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
   
//这里存放数据
return {
     visible: true

};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合 专门存放方法比如点击事件
methods: {
    show () {
        console.log('----------');
        this.visible = false
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
<style lang='stylus' scoped>
.header
   width: 100%
   height: 80px
   background: #0051d6
   .img-top
      position: relative
      width: 1190px
      height: 80px
      margin: 0px 356.5px   
      .header-image
         height: 100%
         
      .delete
         position: absolute
         width: 20px
         right: -10px
      
        
       
       
         
         
         
         
        
   
        
        


</style>