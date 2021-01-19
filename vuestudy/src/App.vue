<template>
  <div id="app">
    <Header msg="Header" />
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Test />
    <Footer msg="Footer" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Test from './components/test.vue'
import Header from './components/default/Header.vue'
import Footer from './components/default/Footer.vue'

export default {
  el: '#app',
  name: 'App',
  components: {
    HelloWorld,
    Test,
    Header,
    Footer
  },
  beforeCreate: function() {
    console.log('beforeCreate');
  },
  created: function() {
    console.log('created');
  },
  mounted: function() {
    console.log('mounted');
    this.msg = 'Hello';
  },
  updated: function() {
    console.log('updated');
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
