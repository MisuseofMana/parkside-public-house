<template>
        <!-- <v-img 
            :src="`/pushpin-${color}.png`"
            width="50"
            height="50"
            class="overlay-image"
        ></v-img> -->
        <v-sheet
        class="mt-5 px-5 pt-5 pb-5 text-center"
        elevation="8"
        height="100%"
        >
        <v-img 
            aspect-ratio="1"
            cover
            :src="`https://foodish-api.com/images/${food}/${food}${image}.jpg`">
        </v-img>
        <p class="mt-3 text-body-1 font-weight-bold ">{{ text }}</p>
        </v-sheet>
</template>

<script setup>
defineProps({
    color: {
        type: String,
        default: 'red'
    },
    text: {
        type: String,
        default: ''
    },
    image: {
        type: Number,
        default: 1,
    },
    food: {
        type: Number,
        default: 1,
    }
})
</script>

<style lang="scss" scoped>
// .overlay-image {
//   position: relative;
//   top: -10px;
//   left: 25px;
//   /* Optional: Center the overlay image */
//   transform: translate(320%, -40%) scaleX(-1);
// }
</style>