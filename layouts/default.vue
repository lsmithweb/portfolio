<template>
  <v-app light>
  <v-toolbar dense fixed app :clipped-left="clipped">
    <v-toolbar-title><nuxt-link to="/" style="text-decoration: none; color: #F66468">LSmith Web</nuxt-link></v-toolbar-title>
    <v-spacer></v-spacer>
    <v-btn
      icon
      @click.stop="drawer = !drawer"
    >
      <v-icon>menu</v-icon>
    </v-btn>
  </v-toolbar>
  <v-navigation-drawer
    fixed
    right
    disable-route-watcher
    enable-resize-watcher
    v-model="drawer"
    app
  >
    <v-list>
      <v-list-tile
        router
        :to="item.to"
        :key="i"
        v-for="(item, i) in items"
        exact
      >
        <v-list-tile-content>
          <v-list-tile-title v-text="item.title"></v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>
    </v-list>
  </v-navigation-drawer>

    <v-content>
        <nuxt />
    </v-content>

  <v-footer :fixed="fixed" app>
    <span>LSmithWeb&copy; 2017</span>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: false,
        fixed: false,
        items: [
          { title: 'Home', to: '/' },
          { title: 'About', to: 'about' },
          { title: 'Services', to: 'services' },
          { title: 'Contact', to: 'contact' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false
      }
    }
  }
</script>
<style lang="stylus">
html, body
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif
  font-size: 100%

main
  min-height: 100vh

</style>
