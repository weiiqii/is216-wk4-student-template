<script setup>
    import { ref } from 'vue'
    const message = ref("Choose your favourite fruit:")
    // const fruit1 = ref("apple")
    // const fruit2 = ref("orange")
    // const fruit3 = ref("peach")

    // Add code here
    // challenge: use array  
    const fruits = ref(["apple", "orange", "peach"])
    
</script>

<template>
    {{ message }} 
   
    <label for=""> <input type="radio" name="fruit"> {{ fruits[0] }} </label> 
    <label for=""> <input type="radio" name="fruit"> {{ fruits[1] }} </label> 
    <label for=""><input type="radio" name="fruit"> {{ fruits[2] }} </label> 

    <!-- <label v-for="fruit in fruits" :key="fruit">
        <input type="radio" name="fruit"> {{ fruit }}
    </label> -->
    
</template>

<style scoped>
</style>
