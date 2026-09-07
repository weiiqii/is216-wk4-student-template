<script setup>
    import { ref } from 'vue'
    // Add code here
    const loginType = ref('username')
    
    
</script>

<template>
    <h1>Please select your login option</h1>
    <select v-model="loginType">
        <option value="username">Username login</option>
        <option value="email">Email login</option>
    </select>
    
    <div v-if="loginType === 'username'">
        <label>Username </label>
        <input placeholder="Enter your username">
    </div>

    <div v-else>
        <label>Email </label>
        <input placeholder="Enter your email address">
    </div>
</template>

