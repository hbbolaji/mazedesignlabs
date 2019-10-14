<template>
  <v-container fluid class="px-8">
    <h1 class="display-2 teal--text my-4 darken-3 text-center">How Can we Help You</h1>
    <h1 class="display-2 teal--text my-4 darken-3 text-center">Get to Know Us More &amp; Hire Us</h1>
    <v-layout row wrap>
      <v-flex xs12 md6>
        <div class="mx-auto py-8">
          <h1 class="text-center teal--text my-8">MEDIA</h1>
          <v-button-navigation>
            <v-btn xs12 text v-for="(nav, index) in navigation" :key="index">
              <span class="teal--text darken-3 text-center" >{{nav.title}}</span>
             </v-btn>
          </v-button-navigation>
        </div>
      </v-flex>
      <v-flex xs12 md6>
        <div class="mx-auto py-8">
          <h1 class="text-center teal--text my-8">SOCIAL</h1>
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
