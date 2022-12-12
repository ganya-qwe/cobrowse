<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome"/>
  <button onclick="TogetherJS(this); return false;">Start TogetherJS</button>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  mounted() {
    let togetherjs = document.createElement('script')
    togetherjs.setAttribute('src', 'https://togetherjs.com/togetherjs-min.js')
    document.head.appendChild(togetherjs)
  },
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
