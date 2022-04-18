<!--
 * @Description: 文件描述
 * @Author: 洛欢
 * @Date: 2022-04-13 17:36:04
 * @LastEditTime: 2022-04-18 14:37:57
 * @LastEditors: 洛欢
-->
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <input type="text" v-model="msg">

    <br /><br />
    <h1>{{ message }}</h1>
    <AInput v-model="message" />

    <br />
    <ACheckbox v-model="ACheckbox" />
    
    <br />
    <Car v-model="index" />
    汽车数量：{{ index }}
  </div>
</template>

<script>
import AInput from './a-input.vue';
import ACheckbox from './a-checkbox.vue';
import Car from './car.vue'

export default {
  name: 'HelloWorld',
  components: {
    AInput,
    ACheckbox,
    Car
  },
  data () {
    return {
      msg: '数据双向绑定',
      message: '自定义组建v-model',
      ACheckbox: true,
      index: 4
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
