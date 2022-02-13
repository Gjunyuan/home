<template>
  <div class="hello">
    123
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  display: block;
  background: #000;
  width: 100%;
  height: 100vh;
}
</style>
