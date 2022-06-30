<template>
  <body>
    <HeaderView/>
    <MainView/>
    <SecondView/>
    <FooterView/>
  </body>
</template>

<script>
import MainView from './components/Main';
import HeaderView from './components/Header';
import SecondView from './components/Second';
import FooterView from './components/Footer';
export default {
  name: 'App',
  components: {
    MainView,
    HeaderView,
    SecondView,
    FooterView,
  },

};
</script>

<style scoped>
 .head {
    opacity: 0.2;
    background-color: black;
 }
</style>
