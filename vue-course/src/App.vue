<template>
  <div id="app">
    <AlertComponent type="primary" text="Primary alert!" />
    <AlertComponent type="secondary" text="Secondary alert!" />
    <AlertComponent type="success" text="Success alert!" />
    <AlertComponent type="danger" text="Danger alert!" />
    <AlertComponent type="warning" text="Warning alert!" />
    <AlertComponent type="info" text="Info alert!" />
    <AlertComponent type="light" text="Light alert!" />
    <AlertComponent type="dark" text="Dark alert!" />
  </div>
</template>

<script>
import AlertComponent from './components/AlertComponent.vue';

export default {
  name: 'App',
  components: {
    AlertComponent
  }
};
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
