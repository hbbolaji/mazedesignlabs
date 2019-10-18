<template>
  <v-container fluid id="about">
    <v-layout row align-center class="my-4 p-8">
      <v-flex xs12 md6 lg6 xl6 class="pr-4">
        <v-img app max-height="300" src="../assets/us.png" aspect-ratio="1" class="mx-8"></v-img>
      </v-flex>
      <v-flex xs12 md6 class="pl-4">
        <div class="mx-8">
          <h1 class="display-1">About Us</h1>
          <p class="">{{about}}</p>
        </div>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      about: 'The Maze Design Lab team is dedicated to providing B2B services, that will help you boost your business. We specialize in providing IT solutions, Accountancy and Finance services, and Marketing services. Shoot us a quick email or text, and see if we can help you meet your business goals!',
    };
  },
};
</script>

<style scoped>
  p {
    line-height: 2.5rem;
  }
</style>
