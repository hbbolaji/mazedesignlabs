<template>
  <div>
    <v-toolbar app fixed color="teal" dark>
      <v-app-bar-nav-icon class="hidden-md-and-up" @click="showNav = !showNav"></v-app-bar-nav-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-toolbar-title>MazeDesignLab</v-toolbar-title>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn v-for="(nav, index) in navigation" :key="index" text>{{nav.title}}</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-navigation-drawer color="teal" fixed temporary app v-model="showNav">
      <v-list dense>
        <v-list-title class="title text-center">
          <h4 class="my-4">MazedesignLabs</h4>
        </v-list-title>
        <v-divider></v-divider>
        <v-list-item v-for="(nav, index) in navigation" :key="index">
          <!-- <v-list-item-icon>
            <v-icon>{{nav.icon}}</v-icon>
          </v-list-item-icon> -->
          <v-list-item-content class="text-center">
            <p>{{nav.title}}</p>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: 'navigation',
  data() {
    return {
      showNav: false,
      navigation: [
        { icon: 'mdi-spotlight', title: 'ABOUT US' },
        { icon: '', title: 'MISSION & VISSION' },
        { icon: '', title: 'OUR SERVICES' },
        { icon: '', title: 'PARTNERS' },
      ],
    };
  },
};
</script>
