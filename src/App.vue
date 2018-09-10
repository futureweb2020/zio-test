<template>
  <div id="app">
    <input type="text" v-model="text"><br/><br/>
    <TextCircle :text="text" />
    <TextCircle :text="text" />
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
