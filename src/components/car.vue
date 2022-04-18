<!--
 * @Description: 文件描述
 * @Author: 洛欢
 * @Date: 2022-04-16 18:01:57
 * @LastEditTime: 2022-04-16 18:22:33
 * @LastEditors: 洛欢
-->
<template>
  <div class="car" @click="handleClick">汽车</div>

  <!-- 父组件通过v-model绑定index到子组件上，而通过v-model绑定的数据在子组件中默认的key是value，所以在props上用value取值，最后通过点击事件执行$emit,而$emit上触发的事件是input，前面我们说过v-model绑定的事件是input，从而在子组件上触发了父组件的input事件，而在触发事件的时候可以传值，所以就实现了父子组件数据双向绑定 -->
</template>
<script>
export default {
  name: 'car',
  props: {
    value: Number
  },
  methods: {
    handleClick() {
      // 执行$emit子组件上触发了父组件的input事件
      this.$emit('input', this.value + 1);
    }
  }
}
</script>

<style scoped>
.car {
  cursor: pointer;
  color: red;
}
</style>
