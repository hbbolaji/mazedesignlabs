<template>
  <v-container fluid>
    <v-layout row wrap align-center class="mx-auto">
      <v-flex>
        <v-col>
          <h1 class="title teal--text darken-4">Maze Design Labs</h1>
          <v-list>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="mb-n4 teal--text">
                  About Us
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="mb-n4 teal--text">
                  Mission and Vision
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="mb-n4 teal--text">Our Services</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="mb-n4 teal--text">Our Partner</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-col>
      </v-flex>
      <v-flex>
        <div>
          <h1 class="teal--text text-center title">Social Media</h1>
          <v-list>
            <v-list-item v-for="(social, index) in socials" :key="index" class="mb-n4">
              <v-list-item-icon>
                <v-icon color="teal">{{social.icon}}</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title class="teal--text">{{social.content}}</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </div>
      </v-flex>
      <v-flex>
        <div>
          <h1 class="teal--text title">Contact Us</h1>
          <v-text-field v-model="label" label="Email"></v-text-field>
          <v-textarea autocomplete="" label="Message"></v-textarea>
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
      ]
    };
  },
};
</script>
