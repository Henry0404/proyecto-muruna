<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Input msg="Bienvenido a Muruna"/>
  </div>
</template>

<script>
import Input from './components/Input.vue'

export default {
  name: 'App',
  components: {
    Input
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
.text-left{
  text-align: left
}
</style>
