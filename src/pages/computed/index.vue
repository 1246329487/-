<!--
 * @Author: yunxi 1246329487@qq.com
 * @Date: 2023-06-10 19:15:20
 * @LastEditors: yunxi 1246329487@qq.com
 * @LastEditTime: 2023-06-29 15:27:41
 * @FilePath: \my-project\src\pages\computed\index.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
  <view> {{ mixTitle }} <children :title="title">
  子组件插槽</children> </view>
</template>

<script>

export default {

  data() {
    return {
      title: "标题",
    };
  },
  methods: {},
  computed: {
    mixTitle() {
      console.log(this.title);
      return this.title + "computed";
    },
  },
};
</script>

<style>
</style>