<template>
  <v-app>
    <Navigation/>
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

export default {
  name: 'App',
  components: {
    Navigation, About, Mission, Partners, Services, Footers,
  },
  data: () => ({
    //
  }),
};
</script>
