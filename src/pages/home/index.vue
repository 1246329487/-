<!--
 * @Author: yunxi 1246329487@qq.com
 * @Date: 2023-06-03 13:06:15
 * @LastEditors: yunxi 1246329487@qq.com
 * @LastEditTime: 2023-06-28 19:21:59
 * @FilePath: \my-project\src\pages\index\index.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
  <view class="content">
    <swiper class="swiper" :indicator-dots="true">
      <swiper-item class="item" item-id="1"> 1 </swiper-item>
      <swiper-item class="item" item-id="2">2 </swiper-item>
      <swiper-item class="item" item-id="3"> 3 </swiper-item>
    </swiper>
    <navigator url="/pages/list/index" open-type="switchTab">
      列表页面12
    </navigator>
    <view v-if="false"> 测试v-if </view>
    <view>
      <input type="text" v-model="title"  />
      <input class="uni-input" focus placeholder="自动获得焦点" />
      {{ title }}
    </view>
  </view>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data() {
    return {
      title: "Hello",
    };
  },
  onLoad() {},
  methods: {},
});
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.swiper {
  width: 750rpx;
  height: 300rpx;
  border: 1px solid red;
}
.item {
  width: 750rpx;
  height: 100rpx;
  border: 1px solid blue;
}
</style>
