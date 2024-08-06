<template>
  <div id="app">
    <header>
      <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/login">Login</router-link>
      </nav>
    </header>
    <main>
      <router-view />
    </main>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App'
})
</script>

<style>
/* 전역 스타일링 */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}

header {
  background-color: #35495e;
  padding: 20px;
}

nav a {
  margin: 0 15px;
  color: white;
  text-decoration: none;
}

nav a.router-link-exact-active {
  font-weight: bold;
}
</style>
