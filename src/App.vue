<template>
  <div id="app">
    <Welcome></Welcome>
  </div>
</template>

<script>
import Welcome from '@/components/Welcome.vue'

export default {
  name: 'App',
  components: {
    Welcome
  }
}
</script>

<style>
body{
  background-image: url('@/assets/img/SG.png');
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
