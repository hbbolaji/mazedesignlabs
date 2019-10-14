<template>
  <v-app>
    <Navigation/>
    <!-- <Landing/> -->
    <About/>
    <Mission/>
    <Services/>
    <Partners/>
    <Footers/>
  </v-app>
</template>

<script>

import Navigation from './components/Navigation';
import Mission from './components/Mission';
import Partners from './components/Partners';
import Services from './components/Services';
import Footers from './components/Footers';
import About from './components/About';
import Landing from './components/Landing';

export default {
  name: 'App',
  components: {
    Navigation, Landing, About, Mission, Partners, Services, Footers,
  },
  data: () => ({
    //
  }),
};
</script>
