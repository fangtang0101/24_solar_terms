<template>
<div class="page_card">
  <div class="back"></div>
  <div class="content">{{name}}</div>
</div>
</template>
<script>
export default {
  // name: 'HelloWorld',
   props: {
      name: String,
    },
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.page_card {
  width: 100px;
  height: 100px;
  line-height: 100px;
}
.back{
   background-color: #DB9019;
    opacity: 0.5;
    display: flex;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 100%;
    z-index: -1;
    border-radius:50px;
    line-height: 100px;
}



</style>
