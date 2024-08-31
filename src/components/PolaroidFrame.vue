<template>
        <v-sheet
            class="px-5 pt-5 pb-5 text-center position-relative"
            elevation="8"
            height="100%"
            rounded="rounded"
        >
        <v-img 
            :aspect-ratio="aspectRatio"
            cover
            :src="getImgUrl(photoName)">
        </v-img>
        <v-img 
            :src="getPinUrl(`pushpin-${props.color}.png`)"
            class="position-absolute pin-shadow top-0 left-0 mt-n6"
            width="96%"
            height="35"
        ></v-img>
        <p class="mt-3 text-body-2 px-10">{{ text }}</p>
        </v-sheet>
</template>

<script setup>

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
    },
    aspectRatio: {
        type: String,
        default: "1",
    }
})

const getImgUrl = (imageNameWithExtension)=> new URL(`/public/pics/${imageNameWithExtension}`, import.meta.url).href;
const getPinUrl = (imageNameWithExtension)=> new URL(`/public/${imageNameWithExtension}`, import.meta.url).href;

</script>

<style>
.pin-shadow {
 -webkit-filter: drop-shadow(4px 4px 4px dimgrey);
 filter: drop-shadow(4px 4px 4px dimgrey);
 transform: rotate(45deg);
}
</style>