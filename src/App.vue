<template>
  <div id="app">
    <header-component class="header-component"/>
    <about-cx/>
    <help-center/>
    <footer-component/>
  </div>
</template>

<script>
import HeaderComponent from './components/Header';
import AboutCX from './components/AboutCX';
import HelpCenter from './components/HelpCenter';
import FooterComponent from './components/Footer';


export default {
  name: 'app',
  components: {
    'header-component': HeaderComponent,
    'about-cx': AboutCX,
    'help-center': HelpCenter,
    'footer-component': FooterComponent
  }
}
</script>

<style lang="scss">
html, 
body {
  height: 100%;
  min-height: 100%;
  width: 100%;
}
</style>

<style lang="scss" scoped>
@import 'App.scss';
</style>
