<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <dev>
    <h4>{{ status }}</h4>
    <a v-for="i in data" :key="i">{{ i }}입니다</a>
  </dev>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
    return{
      status:"안녕하세요 처음뵙겠습니다",
      data:["A","B","C"]
    }
  },
  components: {
    HelloWorld
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
