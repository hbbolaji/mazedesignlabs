<template>
  <v-app>
    <Navigation/>
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

export default {
  name: 'App',
  components: {
    Navigation, Mission, Partners, Services, Footers,
  },
  data: () => ({
    //
  }),
};
</script>
