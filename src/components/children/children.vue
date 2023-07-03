<!--
 * @Author: yunxi 1246329487@qq.com
 * @Date: 2023-06-11 15:57:15
 * @LastEditors: yunxi 1246329487@qq.com
 * @LastEditTime: 2023-07-03 19:29:54
 * @FilePath: \my-project\src\components\children\children.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
  <view @click=""> 公共子组件4   <slot></slot>
      {{ title }}

  </view>
</template>

<script>
export default {
  props: ["title"],
  data() {
    return {
      name:{
        a:1,
        b:2
      }
    };
  },
  methods: {},
  mounted() {
    console.log("测试",this.name);
  },
};
</script>

<style>
</style>