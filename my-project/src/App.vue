<template>
  <div id="app">
    <navigation></navigation>
    <stacked-navigation></stacked-navigation>
  </div>
</template>

<script>
import Navigation from './components/Navigation'
import StackedNavigation from './components/StackedNavigation'

export default {
  name: 'app',
  components: {
    Navigation,StackedNavigation
  }
}
</script>

<style>
body{
  background: #fff;
}
</style>
