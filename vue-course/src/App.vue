<template>
  <div id="app">
    <CardComponent title="First Card" />
    <CardComponent text="How are you?" />
    <CardComponent title="Second Card" text="I'm fine, thank you!" />
  </div>
</template>

<script>
import CardComponent from './components/CardComponent.vue'

export default {
  name: 'App',
  components: {
    CardComponent
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
