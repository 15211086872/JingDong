<!--  -->
<template>
<div class='boot'>
    <img :src="img"/>
      
 
</div>
</template>

<script>
import img from 'styles/QQ图片20190815102039.png'
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';
//import Swiper from "swiper";

export default {
name:'HomeBoot',
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
//这里存放数据
return {
    img: img

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
.boot
   padding: 30px 337.5px 0px 337.5px
   background: #f4f4f4
   width: 100%
   height: 568px
   ma
   .img
      width: 100%

</style>