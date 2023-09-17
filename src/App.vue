<template>
  <div id="app">
  <headerMain></headerMain>
    <router-view/>
  </div>
</template>

<script>
import headerMain from '@/components/headerMain.vue';

export default {
  name: 'App',

  components: {
     headerMain
  },
};
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
ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
}
a {
  text-decoration: none;
}
</style>
