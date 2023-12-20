<template>
  <div>
    <BaseHeader />
  </div>
</template>

<script>
import BaseHeader from './components/Header/BaseHeader.vue'

export default {
  name: 'App',
  components: {
    BaseHeader,
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
}
</style>
