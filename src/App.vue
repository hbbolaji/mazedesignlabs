<template>
  <v-app>
    <Navigation/>
    <Landing/>
    <About/>
    <Mission/>
    <Services/>
    <Partners/>
    <Foots/>
  </v-app>
</template>

<script>

import Navigation from './components/Navigation.vue';
import Mission from './components/Mission.vue';
import Partners from './components/Partners.vue';
import Services from './components/Services.vue';
import Foots from './components/Foots.vue';
import About from './components/About.vue';
import Landing from './components/Landing.vue';

export default {
  name: 'App',
  components: {
    Navigation, Landing, About, Mission, Partners, Services, Foots,
  },
  data: () => ({
    //
  }),
};
</script>
