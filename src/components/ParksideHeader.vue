<template>
    <h1 class="text-h1 d-sr-only">PARKSIDE</h1>
    <v-row class="my-2">
        <v-spacer/>
        <v-col cols="4" sm="3">
            <v-img class="sticker-border" src="/parksidesquareb.png"/>
        </v-col>
        <v-col cols="4" sm="3">
            <v-img class="sticker-border" src="/parksidesquarey.png"/>
        </v-col>
        <v-col cols="4" sm="3">
            <v-img class="sticker-border" src="/parksidesquarer.png"/>
        </v-col>
        <v-spacer/>
    </v-row>
    <v-row align="center">
        <v-col cols="12">
            <v-img class="sticker-border" src="/banner.png"/>
        </v-col>
    </v-row>
    <v-row>
        <v-col cols="12" sm="6" md="6" lg="4" class="text-center">
            <v-sheet elevation="8" class="pa-5" rounded="rounded">
                <p class="text-body-1 mb-2">2608 Shelby St, Indianapolis, IN 46203</p>
                <iframe class="mb-5" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d13124.8222887693!2d-86.14883949839464!3d39.72718534991118!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x886b5bbbaad71cb1%3A0x3dc75f2b6dc9f000!2sParkside%20Public%20House!5e0!3m2!1sen!2sus!4v1724381194904!5m2!1sen!2sus" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                <!-- <p class="text-body-1"><v-icon class="mr-2">mdi-phone</v-icon> (317)000-0000</p> -->
            </v-sheet>
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="8" class="text-center">
            <v-sheet elevation="8" class="pa-5" rounded="rounded">
                <h2 class="text-h2">Open Wed - Sunday</h2>
                <v-table>
                    <tbody>
                    <tr
                        v-for="item in hours"
                        :key="item.day"
                        class="text-body-1"
                    >
                        <td>{{ item.day }}</td>
                        <td>{{ item.hours }}</td>
                    </tr>
                    </tbody>
                </v-table>
            </v-sheet>
        </v-col>
        <v-col cols="12" sm="6" lg="4">
            <PolaroidFrame color="yellow" photo-name="outside.jpg" text="Parkside Public House, Garfield Park's newest place to hang out with a drink and good food."/>
        </v-col>
        <v-col cols="12" sm="6" lg="4">
            <PolaroidFrame color="blue" photo-name="sign.jpg" text="Food, Drinks, Friends. Parkside is all about community, baby."/>
        </v-col>
        <v-col cols="12" sm="6" lg="4" class="text-center">
            <PolaroidFrame color="red" photo-name="skewers.jpg" text="Menu Coming Soon"/>
        </v-col>
        <v-col cols="12" sm="6" lg="4">
            <v-sheet elevation="8" class="pa-5" rounded="rounded">
                <v-img
                src="/pics/gang.jpg"
                class="mb-4"
                />
                <p class="text-body-2">The folks makin' it happen. Pictured center in the apron is Parkside's Manager Josh, a Garfield Park resident and friendly neighborhood gem. </p>
            </v-sheet>
        </v-col>
    </v-row>
</template>

<script setup>
import { ref } from 'vue'
const hours = ref([
    {
        day: 'Monday',
        hours: 'Closed',
    },
    {
        day: 'Tuesday',
        hours: 'Closed',
    },
    {
        day: 'Wednesday',
        hours: '5PM - 10PM',
    },
    {
        day: 'Thursday',
        hours: '5PM - 10PM',
    },
    {
        day: 'Friday',
        hours: '5PM - 10PM',
    },
    {
        day: 'Saturday',
        hours: '10AM - 10PM',
    },
    {
        day: 'Sunday',
        hours: '10AM - 10PM',
    },

])
</script>

<style lang="scss" scoped>
.sticker-border {
 -webkit-filter: drop-shadow(6px 6px 0 white)
         drop-shadow(-6px 6px 0 white)
         drop-shadow(6px -6px 0 white)
         drop-shadow(-6px -6px 0 white);

 filter: drop-shadow(6px 6px 0 white)
         drop-shadow(-6px 6px 0 white)
        drop-shadow(6px -6px 0 white)
        drop-shadow(-6px -6px 0 white);
}
</style>