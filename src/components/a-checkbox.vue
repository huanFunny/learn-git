<!--
 * @Description: 文件描述
 * @Author: 洛欢
 * @Date: 2022-04-16 17:54:02
 * @LastEditTime: 2022-04-18 14:16:26
 * @LastEditors: 洛欢
-->
<template>
  <div class="a-checkbox">
    <!-- 但是像单选框、复选框等类型的输入控件可能会将 value attribute 用于不同的目的。 -->
    <input
      type="checkbox"
      :checked="checked"
      @change="onChange"
    >
  </div>
</template>

<script>
export default {
  name: 'a-checkbox',
  // model 选项可以用来避免这样的冲突
  model: {
    prop: 'checked',
    event: 'change'
  },
  props: {
    checked: Boolean
  },
  methods: {
    onChange (e) {
      this.$emit('change', e.target.checked)
    }
  }
}
</script>