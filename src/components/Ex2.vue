<script setup>
    import { ref } from 'vue'
    const imageSrc = ref('/assets/me.png')
    const imgWidth = ref(200)
    const imgHeight = ref(200)
    const img = {
        src: '/assets/me.png',
        width: 200,
        height: 200
    }
    // Add code here

</script>

<template>

    <!-- Add code here --> 
    <img v-bind:src="imageSrc" :width="imgWidth" :height="imgHeight">
    <img v-bind="img" alt="Profile">
   
</template>
