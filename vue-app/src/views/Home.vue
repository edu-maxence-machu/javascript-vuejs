<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>

    <h2>Articles</h2>

    <ul>
      <li v-for="post in posts" :key="post.id">{{ post.title }}</li>
    </ul>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  methods: {
    async getData() {
      try {
        let response = await fetch("https://my-json-server.typicode.com/typicode/demo/posts");
        this.posts = await response.json();
      } catch (error) {
        console.log(error);
      }
    }
  } ,       
  data() { 
    return {
      posts: [] 
    }
  },
  mounted() { 
        this.getData();
   },
  beforeUnmount() { console.log('Je suis sur le point de disparaître du DOM !') },
  unmounted() { console.log('Je suis supprimé') }
}
</script>
