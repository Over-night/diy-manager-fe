<template>
  <HelloWorld msg="HelloWorld"/>
    <div class="home">
      <h1>Welcome to Our Website!</h1>
      <p>This is the home page of our awesome Vue.js application.</p>
      <button @click="navigateToLogin">Click to Login</button>
      <a>aaaaaaaaaaaaaaaaaaaaaaaaaaaS</a>
    </div>
</template>
  
<script lang="ts">
import { defineComponent } from 'vue'
import { useRouter } from 'vue-router'
import HelloWorld from '../components/HelloWorld.vue';

export default defineComponent({
  name: 'Home',
  components: {
    HelloWorld
  },
  setup() {
    const router = useRouter()

    const navigateToLogin = () => {
      router.push({ name: 'Login' })
    }

    return {
      navigateToLogin,
    }
  }
})
</script>

<style scoped>
.home {
  text-align: center;
  padding: 20px;
}

h1 {
  font-size: 2.5rem;
  color: #42b983;
}

p {
  font-size: 1.2rem;
  color: #35495e;
}

button {
  margin-top: 20px;
  padding: 10px 20px;
  font-size: 1rem;
  color: white;
  background-color: #42b983;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #35495e;
}
</style>
