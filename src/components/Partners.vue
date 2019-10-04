<template>
  <v-container>
    <v-carousel cycle height="600" hide-delimiter-background show-arrows-on-hover delimiter-icon="mdi-checkbox-blank-outline">
    <v-carousel-item v-for="(partner, i) in partners" :key="i">
      <v-sheet color="teal" height="100%">
        <v-row class="fill-height" align="center" justify="center" >
          <div class="display-3 white--text mx-8 my-n8">{{ partner.title }}</div>
          <div class="title white--text text-center mx-4">{{partner.content}}</div>
        </v-row>
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
        { img:'', title: 'SPEED WHEELS', content: 'Speedwheels provides cars for Rental, Purchase and Repair services. They are the only company in Malaysia providing interest free installmnent packages. ', },
        { img:'', title: 'OHJUICE MALAYSIA', content: 'Ohjuice sells premium quality, fresh fruit smoothies that are delicious and healthy.', },
        { img:'', title: 'ROYAL THAI', content: 'Royal Thai Travel and Trading provide memorable tours of Thailand, catering particularly to Muslim tourists. If you are a muslim looking to explore thailand, go with Royal Thai and you won\'t have to worry about looking halal food and family friendly tour spots. ', },
        { img:'', title: 'EDUCAID', content: 'Educaid serves to privde aid in acedamic tasks, particularly with things that might not be in your skillset. They help design diagrams, produce 3D models, and correct language on research papers.', },
      ],
    }
  }
}
</script>
