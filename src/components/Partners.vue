<template>
  <v-container fluid id="partners">
    <v-carousel
      cycle
      height="600"
      hide-delimiter-background
      show-arrows-on-hover
      delimiter-icon="mdi-checkbox-blank-outline">
    <v-carousel-item class="">
      <v-sheet color="teal" height="100%" class="py-16">
        <v-col class="fill-height" align="center" justify="center" >
          <div class="display-3 white--text text-center mb-8">ROYAL THAI</div>
          <v-img
            src="../assets/PartnerLogo/royal-thai.png"
            max-height="250"
            max-width="250">
          </v-img>
          <div class="title white--text text-centers px-8 body-1">{{thai}}</div>
        </v-col>
      </v-sheet>
    </v-carousel-item>
    <v-carousel-item class="">
      <v-sheet color="teal" height="100%" class="py-16">
        <v-col class="fill-height" align="center" justify="center" >
          <div class="display-3 white--text text-center mb-20">SPEED WHEELS</div>
          <v-img
            src="../assets/PartnerLogo/speedwheels.png"
            max-height="250"
            max-width="250"
            class="mb-20">
          </v-img>
          <div class="title white--text text-centers px-8 body-1">{{speed}}</div>
        </v-col>
      </v-sheet>
    </v-carousel-item>
    <v-carousel-item class="">
      <v-sheet color="teal" height="100%" class="py-16">
        <v-col class="fill-height" align="center" justify="center" >
          <div class="display-3 white--text text-center mb-20">OHJUICE MALAYSIA</div>
          <v-img
            src="../assets/PartnerLogo/ohjuice.png"
            max-height="250"
            max-width="250">
          </v-img>
          <div class="title white--text text-centers px-8 body-1">{{juice}}</div>
        </v-col>
      </v-sheet>
    </v-carousel-item>
    <v-carousel-item class="">
      <v-sheet color="teal" height="100%" class="py-16">
        <v-col class="fill-height" align="center" justify="center" >
          <div class="display-3 white--text text-center mb-20">EDUCAID</div>
          <v-img
            src="../assets/PartnerLogo/educaid.png"
            max-height="250"
            max-width="250"
            class="mb-20">
          </v-img>
          <div class="title white--text text-centers px-8 body-1">{{educaid}}</div>
        </v-col>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
  </v-container>
</template>

<script>
export default {
  name: 'partner',
  data() {
    return {
      educaid: 'Educaid serves to privde aid in acedamic tasks, particularly with things that might not be in your skillset. They help design diagrams, produce 3D models, and correct language on research papers.',
      juice: 'Ohjuice sells premium quality, fresh fruit smoothies that are delicious and healthy.',
      speed: 'Speedwheels provides cars for Rental, Purchase and Repair services. They are the only company in Malaysia providing interest free installmnent packages.',
      thai: 'Royal Thai Travel and Trading provide memorable tours of Thailand, catering particularly to Muslim tourists. If you are a muslim looking to explore thailand, go with Royal Thai and you won\'t have to worry about looking halal food and family friendly tour spots.',
    };
  },
};
</script>

<style scoped>
  img {
    background-position: top;
  }
</style>
