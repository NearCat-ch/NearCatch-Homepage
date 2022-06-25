<template>
  <body>
    <HeaderView/>
    <v-app>
      <MainView/>
    </v-app>
  </body>
</template>

<script>
import MainView from './components/Main';
import HeaderView from './components/Header';

export default {
  name: 'App',
  components: {
    MainView,
    HeaderView
  },

};
</script>

<style scoped>
 .head {
    opacity: 0.2;
    background-color: black;
 }
</style>
