<!--
 * @Description: 文件描述
 * @Author: 洛欢
 * @Date: 2022-04-16 17:41:01
 * @LastEditTime: 2022-04-18 14:13:41
 * @LastEditors: 洛欢
-->
<template>
  <div class="a-input">
    <!-- v-model 本质：:value="msg" @input="onInput" -->
    <input v-bind:value="value" @input="onInput"></input>
  </div>
</template>

<script>
export default {
  name: 'a-input',
  props:{
    value: String,
  },
  methods: {
    onInput (e) {
      // $event.target 指代当前触发的事件对象的dom;
      // $event.target.value 就是当前dom的value值;
      var value = e.target.value;
      this.$emit('input', value);
    }
  }
}
</script>