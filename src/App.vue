<template>
  <v-app>

  <AppToolbar></AppToolbar>
  
  <NavigationDrawer></NavigationDrawer>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>

      <!-- If using vue-router -->
      <router-view></router-view>
    </v-container>
  </v-main>

  <v-footer app>
    <!-- -->
  </v-footer>
</v-app>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

<script>
  import NavigationDrawer from '@/components/NavigationDrawer'
  import AppToolbar from '@/components/AppToolbar'

  export default {
    name: 'App',
    components: {
      NavigationDrawer,
      AppToolbar
    }
  }
</script>
