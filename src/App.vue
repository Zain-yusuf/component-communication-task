<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>{{name}}</h1>
    <HelloWorld v-bind:msg="name"/>

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default { 
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      name: "zain"
    }
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
