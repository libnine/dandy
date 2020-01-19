<template>
  <div id="app">
    <headerv/>
    <router-view/>
  </div>
</template>

<script>
import Headerv from '@/components/Headerv'

export default {
  components: {
    'headerv': Headerv
  },

  name: 'App'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat&display=swap');

#app {
  font-family: 'Montserrat';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0C1178;
  margin-top: 40px;
}
</style>
