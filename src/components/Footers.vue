<template>
  <v-container fluid class="px-8">
    <h1 class="display-2 teal--text my-4 darken-3 text-center">How Can we Help You</h1>
    <h1 class="display-2 teal--text my-4 darken-3 text-center">Get to Know Us More &amp; Hire Us</h1>
    <v-layout row wrap>
      <v-flex xs12 md7>
        <div class="mx-auto py-8">
          <h1 class="text-center teal--text title">MEDIA</h1>
          <v-divider class="my-8 teal-text"></v-divider>
          <v-button-navigation class="hidden-sm-and-down">
            <v-btn small xs12 text v-for="(nav, index) in navigation" :key="index">
              <span class="teal--text darken-3 text-center body-1" >{{nav.title}}</span>
             </v-btn>
          </v-button-navigation>
          <v-card class="mx-auto hidden-md-and-up" flat>
            <v-list>
              <v-list-item v-for="(nav, index) in navigation" :key="index">
                <v-list-item-content>
                  <span class="text-center teal--text">{{nav.title}}</span>
                </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-card>
        </div>
      </v-flex>
      <v-flex xs12 md5>
        <div class="mx-auto py-8 mb-16">
          <h1 class="text-center teal--text title">SOCIAL</h1>
          <v-divider class=" my-8"></v-divider>
          <v-botton-navigation>
            <v-btn class="mx-2" fab color="teal" dark small v-for="(social, index) in socials" :key="index">
              <v-icon>{{social.icon}}</v-icon>
            </v-btn>
          </v-botton-navigation>
        </div>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'footer',
  data() {
    return {
      socials: [
        { icon: 'mdi-phone', content: '+60 11 2812 4585' },
        { icon: 'mdi-email', content: 'mazedesignlab@gmail.com' },
        { icon: 'mdi-facebook-box', content: 'Facebook' },
        { icon: 'mdi-twitter-box', content: 'Twitter' },
        { icon: 'mdi-linkedin-box', content: 'Linkedin' },
      ],
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
