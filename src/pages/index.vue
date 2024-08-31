<template>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parkside Public House | Food, Drinks, Friends</title>
    <meta name="description" content="Garfield Park resturaunt located south of Indianapolis, Indiana. Serving food, drinks, and showcasing local art. Focuses on high quality food and atmosphere, cultivating a unique meeting place for locals and visitors alike.">
    <meta property="og:title" content="Parkside Public House | Food, Drinks, Friends">
    <meta property="og:description" content="Garfield Park resturaunt located south of Indianapolis, Indiana. Serving food, drinks, and showcasing local art. Focuses on high quality food and atmosphere, cultivating a unique meeting place for locals and visitors alike.">
    <meta property="og:image" content="https://raw.githubusercontent.com/MisuseofMana/parkside-public-house/main/outside.jpg">
    <meta property="og:url" content="https://www.parksidepublichouse.com">
    <meta property="og:type" content="website">
    <meta property="og:site_name" content="Parkside Public House">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="Parkside Public House">
    <meta name="twitter:description" content="Garfield Park resturaunt located south of Indianapolis, Indiana. Serving food, drinks, and showcasing local art. Focuses on high quality food and atmosphere, cultivating a unique meeting place for locals and visitors alike.">
    <meta name="twitter:image" content="https://www.parksidepublichouse.com">
  </head>
  <v-row>
    <v-col cols="12" sm="6" class="pb-15 mb-10">
      <PolaroidFrame color="red" photo-name="bites.jpg" text="Brunch from 10am - 3pm"/>
      <v-btn href="/menu/brunch.pdf" target="_blank" color="#2a95a3" size="x-large" width="100%" class="mt-4">Get the Brunch Menu</v-btn>
    </v-col>
    <v-col cols="12" sm="6" class="pb-15 mb-10">
      <PolaroidFrame color="blue" photo-name="skewers.jpg" text="Snacks from 4PM to 5PM : Dinner 5PM - 10PM"/>
      <v-btn href="/menu/dinner.pdf" target="_blank" color="#fdbe15" size="x-large" width="100%" class="mt-4">Get the Dinner Menu</v-btn>
    </v-col>
    <v-col cols="12" sm="6" md="6" lg="4">
        <PolaroidFrame color="yellow" photo-name="outside.jpg" text="Garfield Park's newest place to hang out with a drink and good food."/>
    </v-col>
    <v-col cols="12" sm="6" md="6" lg="4">
        <PolaroidFrame color="red" photo-name="gallery.jpg" text="Local art to admire while you dine in."/>
    </v-col>
    <v-col cols="12" sm="6" md="6" lg="4">
        <PolaroidFrame color="blue" photo-name="sign.jpg" text="Food, Drinks, Friends. Parkside is all about community, baby."/>
    </v-col>
    <v-col cols="12" sm="12" md="6" lg="8">
        <PolaroidFrame color="yellow" aspect-ratio="1.9" photo-name="gang.jpg" text="The folks makin' it happen."/>
    </v-col>
    <v-col cols="12">
      <v-sheet elevation="8" class="pa-10 py-5" rounded="rounded">
        <v-row class="d-flex justify-center align-center">
          <v-col cols="12" sm="3" md="4">
            <v-img src="/parkside-logo.png"/>
          </v-col>
          <v-col cols="12" sm="9" md="8">
            <h2 class="text-h2 mb-5"> The Story</h2>
            <p class="mb-2 text-body-2">Welcome to Parkside, friends!</p>
            <p class="mb-2 text-body-2">Every great story has a beginning, and ours starts with this neighborhood - Garfield Park.  We moved to Garfield Park several years ago and were immediately welcomed into the community with open arms.  We fell in love with our neighborhood because it is one of the most inviting, creative communities in Indianapolis.  Parkside seeks to embody that same spirit!</p>

            <p class="mb-2 text-body-2">We aren't a regular public house. We're a cool public house.  Parkside is a restaurant, a watering hole, a community gathering place, an art space, and an evolving project. We have fun in the kitchen, with a rotating menu driven by Fidelmar Garcia Garcia and Abbi Merriss. We curate our beers and wines (don't worry - we got Old Style for our fellow degenerates).  We collaborate with the two art galleries on site. Come enjoy imbibes alongside neighbors and help us create a space that captures the cultural zeitgeist of Indianapolis!</p>

            <h3 class="text-h4 text-right">-Josh Haines</h3>
          </v-col>
        </v-row>
        </v-sheet>
    </v-col>
  </v-row>

  <v-row>
    <v-col cols="12">
      <v-sheet elevation="8" class="pa-10 pr-5 py-5" rounded="rounded">
        <v-row class="d-flex justify-center align-center">
          <v-col cols="12">
            <v-img width="50px" height="50px" src="/yellow-stars.png"/>
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
        </v-row>
        </v-sheet>
    </v-col>
  </v-row>

  <v-row v-if="false">
    <v-col cols="12">
      <v-sheet elevation="8" class="pa-10 pr-5 py-5 text-body-2 mb-6" rounded="rounded">
         <h2 class="text-h2">
          Send Us A Message
         </h2>
         <p class="text-body-2 mb-2">Reach out to say hi, or give us feedback directly! Feel free to send suggestions or just drop us a line.</p>
      </v-sheet>
      <v-form>        
      <v-row>
          <v-col cols="12" md="6">
            <v-text-field class="text-body-2 elevation-8" hide-details label="Your Name" variant="solo"></v-text-field>
          </v-col>
          
          <v-col cols="12" md="6">
            <v-text-field class="text-body-2 elevation-8" hide-details label="Your Email Address" variant="solo"></v-text-field>
          </v-col>

          <v-col>
            <v-textarea class="text-body-2 elevation-8" hide-details label="What's on your mind?" variant="solo"></v-textarea>
          </v-col>
      </v-row>
      <v-row>
        <v-spacer/>
        <v-col cols="12" md="5">
          <v-btn type="submit" color="info" size="x-large" width="100%" text="Send It!"></v-btn>
        </v-col>
      </v-row>
      </v-form>
    </v-col>
  </v-row>

  <v-row>
    <v-col cols="4">
      <v-img src="/yellow-star.png"></v-img>
    </v-col>
    <v-col cols="4">
      <v-img src="/yum-cloud.png"></v-img>
    </v-col>
    <v-col cols="4">
      <v-img src="/red-stars.png"></v-img>
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

<style>
.flip-hor {
  -webkit-transform: scaleX(-1);
  transform: scaleX(-1);
}
</style>
