<template>
  <nav>
    <v-app-bar
      flat
      app>
      <v-app-bar-nav-icon
        class="grey--text"
        @click="drawer = !drawer">
      </v-app-bar-nav-icon>
      <v-toolbar-title class="text-uppercase grey--text">
        <span class="font-weight-light">Todo</span>
        <span>Junya</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn color="grey">
        <span>Sign Out</span>
        <v-icon>mdi-login</v-icon>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      app
      class="success">
      <v-list>
        <v-list-item
          v-for="link in links"
          :key="link.text"
          :to="link.route">
          <v-list-item-action>
            <v-icon class="white--text">{{ link.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title class="white--text font-weight-medium">{{ link.text }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

  </nav>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      links: [
        { icon: 'mdi-apps-box', text: 'Dashboard', route: '/' },
        { icon: 'mdi-folder', text: 'My Projects', route: '/projects' },
        { icon: 'mdi-account ', text: 'Team', route: '/team' },
      ]
    }
  }
}
</script>
