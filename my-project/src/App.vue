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
import SoftwareDevelopmentPlan from './components/SoftwareDevelopmentPlan'

export default {
  name: 'app',
  components: {
    Navigation,StackedNavigation,SoftwareDevelopmentPlan
  }
}
</script>

<style>
body{
  background: #fff;
}
</style>
