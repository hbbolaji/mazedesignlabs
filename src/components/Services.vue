<template>
  <v-container>
    <v-layout row wrap justify-center>
      <v-flex justify-center xs12 md4 v-for="(service, index) in services" :key="index">
        <div>
          <v-avatar color="teal lighten-5" size="150" class="text-center mb-4">
            <v-icon x-large color="teal">{{service.icon}}</v-icon>
          </v-avatar>
          <h2 class="headline mb-4 text-xs-center">{{service.title}}</h2>
          <p>{{service.content}}</p>
        </div>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'service',
  data() {
    return {
      services: [
        { icon: 'mdi-code-braces', title: 'WEB DEVELOPMENT', content: 'Have your business on the greatest marketing platform (internet), with your style. Showcase what makes your product the best option witha style to match', },
        { icon: 'mdi-pencil', title: 'GRAPHIC DESIGNING', content: 'Make use of beautiful designs to promote your products and services in the most effective way.', },
        { icon: 'mdi-desktop-mac', title: 'PRODUCT DESIGNING', content: 'Make your products stand out with designs that would make your potential customers choose to buy your products.', },
        { icon: 'mdi-home-modern', title: 'CREATING MARKET CONTENT', content: 'Make effective use of our marketing strategies to boost your sales or tap in to new markets with offline and online marketing', },
        { icon: 'mdi-thumb-up-outline', title: 'SOCIAL MEDIA MANAGEMENT', content: 'Connect with your clients and boost sales with the aid of effective soical media presence.', },
        { icon: 'mdi-cash', title: 'FINANCIAL ADVISORY', content: 'Understand where the financial standing of your business with the aid of our professional financial analyst to improve your businesses financial efficiency or to convince potential investors why your business is on a course to succeed', },
      ],
    }
  },
}
</script>
