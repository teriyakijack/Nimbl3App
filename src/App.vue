<template lang="jade">
  .container
    Drawer
    router-view
</template>

<script>
import Drawer from './components/Drawer'
import Hello from './components/Hello'
import Order from './components/Order'

export default {
  name: 'app',
  components: {
    Drawer,
    Hello,
    Order
  }
}
</script>

<style lang="sass">

  html,
  body
    margin: 0
    padding: 0
    
  .container
    display: flex
    height: 100vh

    .drawer
      flex: 1

    .hello
      flex: 2
      background-color: black
    
</style>
