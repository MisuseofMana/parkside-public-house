<template>
  <v-app>
    <v-main class="background-image">
      <v-container>
        <ParksideHeader/>
        <router-view/>
        <AppFooter/>
      </v-container>
      </v-main>
  </v-app>
</template>

<script setup>
</script>

<style>
  .background-image {
    background: url('/corkboard.jpg') repeat;
    min-height: 100vh;
    min-width: 100vw;
  }
</style>
