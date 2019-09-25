<template>
  <v-app>
    <v-toolbar app>
      <v-app-bar-nav-icon @click="showNav = !showNav"></v-app-bar-nav-icon>
      <v-toolbar-title>MazeDesignLab</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn v-for="(nav, index) in navigation" :key="index" text>{{nav.title}}</v-btn>
      </v-toolbar-items>
      <v-navigation-drawer absolute temporary app v-model="showNav">
        <v-list dense>
          <v-list-item v-for="(nav, index) in navigation" :key="index">
            <v-list-item-icon>
              <v-icon>{{nav.icon}}</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              {{nav.title}}
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
    </v-toolbar>
    
  </v-app>
</template>

<script>
export default {
  name: 'navigation',
  data() {
    return {
      showNav: false,
      navigation: [
        {icon: '', title: 'ABOUT US',},
        {icon: '', title: 'MISSION & VISSION',},
        {icon: '', title: 'OUR SERVICES',},
        {icon: '', title: 'PARTNERS',},
      ]
    }
  }
}
</script>