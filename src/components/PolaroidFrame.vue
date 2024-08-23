<template>
        <v-sheet
        class="px-5 pt-5 pb-5 text-center position-relative"
        elevation="8"
        height="100%"
        rounded="rounded"
        >
        <v-img 
            aspect-ratio="1"
            cover
            :src="getImgUrl(photoName)">
        </v-img>
        <v-img 
            :src="getPinUrl(`pushpin-${props.color}.png`)"
            class="position-absolute top-0 left-0 mt-n5"
            width="96%"
            height="35"
        ></v-img>
        <p class="mt-3 text-body-2">{{ text }}</p>
        </v-sheet>
</template>

<script setup>
import { computed } from 'vue'

const props = defineProps({
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
    photoName: {
        type: String,
        default: '',
    }
})

const getImgUrl = (imageNameWithExtension)=> new URL(`/public/pics/${imageNameWithExtension}`, import.meta.url).href;
const getPinUrl = (imageNameWithExtension)=> new URL(`/public/${imageNameWithExtension}`, import.meta.url).href;

</script>