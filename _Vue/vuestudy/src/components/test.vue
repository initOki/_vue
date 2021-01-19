<template>
  <div class="hello">
    <span>helloworld</span>
  </div>
</template>

<script>
  export default {
    name: 'Test',
    props: {
      msg: String
    }
  }
</script>

<style scoped>
  .hello {
    font-size: 16px;
    color: red;
  }
</style>