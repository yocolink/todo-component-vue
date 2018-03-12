<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
    TODO MAISON
    <todo/>
    ------
    TODO TRAVAIL
    <todo/>
    ------
    TODO FETE
    <todo/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import todo from './components/todo'

export default {
  name: 'App',
  components: {
    HelloWorld,
    todo
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
