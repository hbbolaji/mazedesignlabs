<template>
  <v-container fluid>
    <v-layout row align-center class="px-8">
      <v-flex xs12 md6 lg6 xl6>
        <div class="mx-8 mt-4">
          <p v-for="(mission, index) in missionContent" :key="index" :class="mission.size">{{mission.title}}</p>
        </div>
      </v-flex>
      <v-flex xs12 md6>
        <v-img src='../assets/mission.png' max-height="250px" aspect-ratio="1" class="mx-8 mt-4"></v-img>
      </v-flex>
      <v-flex xs12 md6>
        <v-img src="../assets/vision.png" max-height="250px" aspect-ratio="1" class="mx-8 mt-4"></v-img>
      </v-flex>
      <v-flex xs12 md6>
        <div class="mx-8 mt-4">
          <p class="" v-for="(vision, index) in visionContent" :key="index" :class="vision.size">{{vision.title}}</p>
        </div>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'mission',
  data() {
    return {
      missionContent: [
        { title: 'Mission', size: 'display-1', align: 'text-xs-center' },
        { title: 'To provide high-quality, cost-effective and highly beneficial consultancy to good businesses', size: 'body-1'},
        { title: 'To provide effective solutions with the help of experts', size: 'body-1' },
        { title: 'To benefit society by supporting and helping good businesses grow.', size: 'body-1'  },
      ],
      visionContent: [
        { title: 'Vision', size: 'display-1', align: 'text-md' },
        { title: 'To be the leading business consultancy company with consistent and high-quality client support.', size: 'body-1'  },
        { title: 'To develop a wide and diversified web of resource network in order to allow businesses to produce high-quality products and provide high-quality services', size: 'body-1'  },
      ],
    };
  },
};
</script>

<style scoped>
  p {
    line-height: 2rem;
    text-align: justify;
  }
</style>
