<template>
    <header class="bg-gray-800 text-lime-500 p-4 flex justify-between items-center">
      <div class="text-2xl font-bold">
        <router-link to="/" class="text-white">DIY Manager</router-link>
      </div>
      <nav class="space-x-4">
        <router-link to="/" class="hover:text-gray-300">Home</router-link>
        <router-link to="/about" class="hover:text-gray-300">About</router-link>
        <router-link to="/contact" class="hover:text-gray-300">Contact</router-link>
      </nav>
      <div>
        <router-link to="/login" class="hover:text-gray-300">Login</router-link>
      </div>
    </header>
</template>
  
<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Navbar',
})
</script>
  