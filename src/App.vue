<template>
  <div id="app">
    <Header/>
    <Footer/>
    <!--<img src="./assets/logo.png">-->
    <!--<HelloWorld/>
    <Test/>-->

  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld'
//import Test from './components/test'
import Header from './components/header'
import Footer from './components/footer'


export default {
  name: 'App',
  components: {
    Header,
    Footer
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
