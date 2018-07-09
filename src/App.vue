<template>
  <div id="app">
    <!--v-text:从data中绑定的text文本,是元素的innerText只能在双标签中使用-->
    <!--v-html: 是元素的innerHtml，不能包含{{}}-->
    <!--v-if v-show :是否隐藏-->
    <!--v-model :双向绑定，页面与内存双向改变-->
    <!--v-bind  : 单项绑定，内存可以改变页面，页面可以改变内存-->
    <!--<img src="./assets/logo.png">-->
    <!--<router-view/>-->
    <span v-text="text"></span>
    <input/>
    <span v-html="html"></span>
    <div v-if="ifShow" style="height: 300px;background-color: red"></div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      text: '绑定的text',
      html: '<ul> <li>111</li><li>222</li></ul>',
      ifShow: false
    }
  }
}
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
