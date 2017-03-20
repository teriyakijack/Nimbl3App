<template lang="jade">
  aside.drawer.drawer-container
    .drawer-header
      img(src="static/icons/logo-white.svg")
    .drawer-menu
      router-link(to="/", tag="div", active-class="active", exact).drawer-menu-item
        i.icons-dashboard
        p Dashboard
      router-link(to="/Order", tag="div", active-class="active").drawer-menu-item
        i.icons-cart
        p Orders
      router-link(to="/Companies", tag="div", active-class="active").drawer-menu-item
        i.icons-factory
        p Companies
        i.icons-arrow
      router-link(to="/Products", tag="div", active-class="active").drawer-menu-item
        i.icons-box
        p Products
      router-link(to="/Documents", tag="div", active-class="active").drawer-menu-item
        i.icons-document
        p Documents
      router-link(to="/Pricing", tag="div", active-class="active").drawer-menu-item
        i.icons-price
        p Pricing
      router-link(to="/Brands", tag="div", active-class="active").drawer-menu-item
        i.icons-shape
        p Brands
      router-link(to="/Settings", tag="div", active-class="active").drawer-menu-item
        i.icons-gear
        p Settings
        i.icons-arrow
      router-link(to="/Reports", tag="div", active-class="active").drawer-menu-item
        i.icons-chart
        p Reports
      router-link(to="/Users", tag="div", active-class="active").drawer-menu-item
        i.icons-people
        p Account Users
    .drawer-footer
      p POWERED BY
      img(src="static/icons/logo-white.svg")
</template>

<script>
export default {
  name: 'drawer'
}
</script>
<style lang="sass" scoped>
  @import '../assets/sass/common.sass'

  .drawer-container
    background-color: $light-purple
    max-width: 246px
    display: flex
    flex-direction: column

    p
      margin: 0
      color: $bright-purple
      font-size: 14px
      font-weight: 600
      letter-spacing: 1px

    .drawer-header
      background-color: $dark-purple
      display: flex
      justify-content: center
      align-items: center
      
      img
        width: 158px
        height: 50px
        margin: 10px auto

    .drawer-menu
      background-color: $light-purple
      overflow-x: hidden
      overflow-y: auto
      flex: 1
      
      .drawer-menu-item
        display: flex
        justify-content: center
        align-items: center
        height: 66.87px
        
        i
          flex: 1

        p
          flex: 2

        &.active
          background-color: $almost-dark-purple
          box-shadow: 0 -1px 0 0 #4C1367, 0 1px 0 0 #4C1367

          p
            color: $pure-white !important

    .drawer-footer
      display: flex
      flex-direction: column
      justify-content: center
      align-items: center
      padding: 22px 0

      p
        font-size: 11px

      img
        width: 113px
        height: 36px
</style>
