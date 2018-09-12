<template>
  <div id="app">
    <input type="text" v-model="text"><br/><br/>
    <TextCircle :text="text" :size="100" :centerX="200" :centerY="150" bgColor="green" />
    <TextCircle :text="text" :size="150" :centerX="200" :centerY="300" bgColor="lightgreen" />
  </div>
</template>

<script>
import TextCircle from './components/TextCircle.vue'

export default {
  name: 'app',
  components: {
    TextCircle
  },
  data: function () {
    return {
      text: ''
    }
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
