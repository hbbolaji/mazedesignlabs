<template>
  <v-container fluid>
    <v-carousel cycle height="600" hide-delimiter-background show-arrows-on-hover delimiter-icon="mdi-checkbox-blank-outline">
    <v-carousel-item v-for="(partner, index) in partners" :key="index" class="">
      <v-sheet color="teal" height="100%" class="py-16">
        <v-col class="fill-height" align="center" justify="center" >
          <div class="display-3 white--text text-center mb-20">{{ partner.title }}</div>
          <v-img class="mb-20" :src="partners[index].img" max-height="250" max-width="250"></v-img>
          <div class="title white--text text-centers px-16">{{partner.content}}</div>
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
      partners: [
        { img: '../assets/PartnerLogo/speedwheels.png', title: 'SPEED WHEELS', content: 'Speedwheels provides cars for Rental, Purchase and Repair services. They are the only company in Malaysia providing interest free installmnent packages. ' },
        { img: '../assets/PartnerLogo/ohjuice.png', title: 'OHJUICE MALAYSIA', content: 'Ohjuice sells premium quality, fresh fruit smoothies that are delicious and healthy.' },
        { img: '../assets/PartnerLogo/royal-thai.png', title: 'ROYAL THAI', content: 'Royal Thai Travel and Trading provide memorable tours of Thailand, catering particularly to Muslim tourists. If you are a muslim looking to explore thailand, go with Royal Thai and you won\'t have to worry about looking halal food and family friendly tour spots. ' },
        { img: '../assets/PartnerLogo/educaid.png', title: 'EDUCAID', content: 'Educaid serves to privde aid in acedamic tasks, particularly with things that might not be in your skillset. They help design diagrams, produce 3D models, and correct language on research papers.' },
      ],
    };
  },
};
</script>

<style scoped>
  img {
    background-position: top;
  }
</style>
