<template>
  <div id="app">
    <navigation></navigation>
    <stacked-navigation></stacked-navigation>
    <software-development-plan></software-development-plan>
  </div>
</template>

<script>
import Navigation from './components/Navigation'
import StackedNavigation from './components/StackedNavigation'
import SoftwareDevelopmentPlan from './components/developmentPlan/SoftwareDevelopmentPlan'

export default {
  name: 'app',
  components: {
    Navigation,StackedNavigation,SoftwareDevelopmentPlan
  }
}
</script>

<style>
body{
  /* background: #fff; */
  background: #fff;
  background-color:rgba(255,255,255,0.2); 
  background-size: 100% 100%;
  background-image: url('./assets/img/dev-bg.jpg');
  background-repeat:no-repeat;
  background-attachment: fixed;
  
}
</style>
