<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div id="mount-point"></div>
  </div>


</template>

<script>
  import Vue from 'vue'
export default {
  name: 'helloWorld',
  data(){
    return{
      msg: '欢迎来到菜鸟教程！'
    }
  }
}

// 创建构造器
var Profile = Vue.extend({
  template: '<p>{{firstName}} {{lastName}} aka {{alias}}</p>',
  data: function () {
    return {
      firstName: 'Walter',
      lastName: 'White',
      alias: 'Heisenberg'
    }
  }
})
// 创建 Profile 实例，并挂载到一个元素上。
new Profile().$mount('#mount-point')
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
