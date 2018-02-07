<template>
<div>
二十四节气
<!-- <h4 class="" v-for='item in list'>{{item}}</h4> -->
<div v-for='item in list'>
  <card :name="item"> </card>
</div>

<!--  <flat-surface-shader type="webgl" 
                         :light="{ambient: '#BD9019', diffuse: '#F1AAA6'}"
                         width=2000
                         class = "flat"
                         height=1000>
    </flat-surface-shader>

      <flat-surface-shader class="shader"
                         type="canvas" 
                         :light="{ambient: '#BD9019', diffuse: '#F1AAA6', draw: false}" 
                         :mesh="{segments: 1, slices: 1, width: 1.8, height: 1.8}">
    </flat-surface-shader> -->

</div>
</template>

<script>

import card from './card'

export default {
  components:{ 'card':card},
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      list:['立春','雨水','惊蛰','春分','清明','谷雨','立夏','小满','芒种','夏至','小暑','大暑','立秋','处暑','白露','秋分','寒露','霜降','立冬','小雪','大雪','冬至','小寒','大寒']
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.shader {
      width: 100vw;
      height: 100vh;
  }

.flat{
  width: 100px;
  height: 100px;
  position: fixed;
  top: 20px;
  left: 700px;
  z-index: -1;
}

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
