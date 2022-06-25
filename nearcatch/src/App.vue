<template>
  <body>
    <HeaderView/>
    <MainView/>
    <SecondView/>
  </body>
</template>

<script>
import MainView from './components/Main';
import HeaderView from './components/Header';
import SecondView from './components/Second'
export default {
  name: 'App',
  components: {
    MainView,
    HeaderView,
    SecondView,
  },

};
</script>

<style scoped>
 .head {
    opacity: 0.2;
    background-color: black;
 }
</style>
