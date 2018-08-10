<template>
  <div id="app">
      <Skills msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import Skills from './components/Skills.vue'

export default {
  name: 'app',
  components: {
    Skills
  }
}
</script>

<style>
  body{
    background-color: #eeeeee ;
  }
</style>
