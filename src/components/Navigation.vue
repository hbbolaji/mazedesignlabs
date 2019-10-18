<template>
  <div>
    <v-app-bar dense fixed app color="teal" dark>
      <v-app-bar-nav-icon class="hidden-md-and-up" @click="showNav = !showNav"></v-app-bar-nav-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-toolbar-title>MazeDesignLab</v-toolbar-title>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn
          v-for="(nav, index) in navigation"
          :key="index"
          :href="nav.href"
          text>
          {{nav.title}}
        </v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-navigation-drawer dark z-index=0 color="teal" fixed temporary app v-model="showNav">
      <v-list dense>
        <v-list-item class="title text-center">
          <v-list-item-content>
            <h4 class="my-4 text-white">MazedesignLabs</h4>
          </v-list-item-content>
        </v-list-item>
        <v-divider></v-divider>
        <v-list-item v-for="(nav, index) in navigation" :key="index">
          <!-- <v-list-item-icon>
            <v-icon>{{nav.icon}}</v-icon>
          </v-list-item-icon> -->
          <v-list-item-content class="text-center">
            <v-btn text :href="nav.href" class="text-white">{{nav.title}}</v-btn>
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
        { icon: 'mdi-spotlight', title: 'ABOUT US', href: '#about' },
        { icon: '', title: 'MISSION & VISSION', href: '#mission' },
        { icon: '', title: 'OUR SERVICES', href: '#services' },
        { icon: '', title: 'PARTNERS', href: '#partners' },
        { icon: '', title: 'CONTACT US', href: '#contact' },
      ],
    };
  },
};
</script>
