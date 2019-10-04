<template>
  <v-container grid-list-md>
    <v-layout row align-center>
      <v-flex xs12 md6>
        <div>
          <p v-for="(mission, index) in missionContent" :key="index" :class="mission.size">{{mission.title}}</p>
        </div>
      </v-flex>
      <v-flex xs12 md6>
        <div>
          <p v-for="(vision, index) in visionContent" :key="index" :class="vision.size">{{vision.title}}</p>
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
        { title: 'Mission', size: 'display-1', align: 'text-xs-center'},
        { title: 'To provide high-quality, cost-effective and highly beneficial consultancy to good businesses', },
        { title: 'To provide effective solutions with the help of experts', },
        { title: 'To benefit society by supporting and helping good businesses grow.', },
      ],
      visionContent: [
        { title: 'Vision', size: 'display-1', align: 'text-md'},
        { title: 'To be the leading business consultancy company with consistent and high-quality client support.', },
        { title: 'To develop a wide and diversified web of resource network in order to allow businesses to produce high-quality products and provide high-quality services', },
      ],
    }
  }
}
</script>

<style scoped>
</style>
