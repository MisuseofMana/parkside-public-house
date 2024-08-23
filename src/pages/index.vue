<template>
  <v-row align="center">
    <v-col cols="4" md="3" lg="3" xl="3" v-for="(link, index) in stuff" :key="link">
      <PolaroidFrame :color="colors[index%3]" :food="food[index%3]" :text="link" :image="index + 1" />
    </v-col>
  </v-row>
  <v-row>
    <v-col cols="12">
      <v-sheet elevation="8" class="pr-10 py-5" rounded="rounded">
        <v-row class="d-flex justify-center align-center">
          <v-col cols="4">
            <v-img src="/parkside-logo.png"/>
          </v-col>
          <v-col cols="8">
            <h2 class="text-h2 mb-5"> The Story</h2>
            <p class="mb-2 text-body-2">Welcome to Parkside, friends!</p>
            <p class="mb-2 text-body-2">Every great story has a beginning, and ours starts with this neighborhood - Garfield Park.  We moved to Garfield Park several years ago and were immediately welcomed into the community with open arms.  We fell in love with our neighborhood because it is one of the most inviting, creative communities in Indianapolis.  Parkside seeks to embody that same spirit!</p>

            <p class="mb-2 text-body-2">We aren't a regular public house. We're a cool public house.  Parkside is a restaurant, a watering hole, a community gathering place, an art space, and an evolving project. We have fun in the kitchen, with a rotating menu driven by Fidelmar Garcia Garcia and Abbi Merriss. We curate our beers and wines (don't worry - we got Old Style for our fellow degenerates).  We collaborate with the two art galleries on site. Come enjoy imbibes alongside neighbors and help us create a space that captures the cultural zeitgeist of Indianapolis!</p>

            <h3 class="text-h4 text-right">~Josh Haines</h3>
          </v-col>
        </v-row>
        </v-sheet>
    </v-col>
  </v-row>

  <v-row>
    <v-col cols="12">
      <v-sheet elevation="8" class="pl-10 pr-5 py-5" rounded="rounded">
        <v-row class="d-flex justify-center align-center">
          <v-col cols="8">
            <h2 class="text-h2 mb-5">The Gang</h2>
            <p class="mb-2 text-h5">Josh Haines - Owner and General Manager</p>
            <p class="mb-5 text-body-2">Josh is the master of ceremonies, an artist, and all around silly goose.  He has been involved with several projects in the neighborhood -  including starting Garfield Brewery and helping create the Garfield Park Art and Music Festival.  Some ask why he can't just take a break every now and then, and to that he says no firmly, but politely.</p>
            
            <p class="mb-2 text-h5">Phil Kirk - Owner</p>
            <p class="mb-5 text-body-2">Phil is a renaissance man - a realtor, an interior designer, a vampire????, and other mysterious things.  Phil is a co-owner of the Yoke Pavillion who has spent the better part of two years transforming the space!  He's got BIG DREAMS - BIG DREAMS FOR THIS NEIGHBORHOOD.</p>
            
            <p class="mb-2 text-h5">Fidelmar Garcia Garcia - Chef</p>
            <p class="mb-5 text-body-2">What can we say about Fidel?  He's a romantic at heart, and food is his love language and cooking is the dance.  To Fidel, there is just good food.  He's been everywhere from the best local breakfast joint, Ruth's Cafe to bangers like Union 50 and The Skyline Club. Fidel cooks with passion, and cooks to connect.</p>
            
            <p class="mb-2 text-h5">Abbi Merriss - Chef</p>
            <p class="mb-5 text-body-2">Abbi is the culinary maven behind Bluebeard!  A pure creative force that entwines narrative, taste, and aesthetic, Abbi also enjoys gardening with her dog Boogie.  Does she have a constant stream of energy from her undiagnosed ADHD? Yes.  Does she make a knee-slapper of a meal? Also yes.</p>
          </v-col>
          <v-col cols="4">
            <v-img src="/yellow-stars.png"/>
          </v-col>
        </v-row>
        </v-sheet>
    </v-col>
  </v-row>

  <!-- <v-row>
    <v-col cols="12">
      <v-sheet elevation="8" class="pl-10 pr-5 py-5" rounded="rounded">
        <v-row class="d-flex justify-center align-center">
          <v-col cols="8">
            <h2 class="text-h2 mb-5"> The Menu </h2>
          </v-col>
          <v-col cols="4">
            <v-img src="/yum-cloud.png"/>
          </v-col>
        </v-row>
        </v-sheet>
    </v-col>
  </v-row>

  <v-row>
    <v-col cols="12">
      <v-sheet elevation="8" class="pl-5 pr-10 py-5" rounded="rounded">
        <v-row class="d-flex justify-center align-center">
          <v-col cols="4">
            <v-img src="/yellow-star.png"/>
          </v-col>
          <v-col cols="8">
            <h2 class="text-h2 mb-5"> The Galleries </h2>
            <p>Link to Imagine Indy</p>
          </v-col>
        </v-row>
        </v-sheet>
    </v-col>
  </v-row>

  <v-row>
    <v-col cols="12">
      <v-sheet elevation="8" class="pl-10 pr-5 py-5" rounded="rounded">
        <v-row class="d-flex justify-center align-center">
          <v-col cols="8">
            <h2 class="text-h2 mb-5"> The Happenings </h2>
            <p>We need to get this plane off the ground and flying! Check back in the fall for our first events!</p>
          </v-col>
          <v-col cols="4">
            <v-img src="/parksidesquarer.png"/>
          </v-col>
        </v-row>
        </v-sheet>
    </v-col>
  </v-row> -->

</template>

<script setup>
  import { ref } from 'vue'
  const colors = ref([
    'blue',
    'yellow',
    'red'
  ])
  const food = ref([
    'burger',
    'rice',
    'butter-chicken'
  ])
  const stuff = ref([
    // 'The Menu',
    // 'The Story',
    // 'The Gang',
    // 'The Galleries',
    // 'Happenings',
    // 'Get With Us'
  ])
</script>

<style>
.flip-hor {
  -webkit-transform: scaleX(-1);
  transform: scaleX(-1);
}
</style>
