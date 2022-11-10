<template>
  <div id="app">
    <AppHeader />

  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import AppHeader from "@/components/AppHeader";


export default {
  name: 'App',
  components: {
      AppHeader
  }
}
</script>

<style>
@font-face {
  font-family: "spotify";
  src: url('./fonds/Spotify-Font/GothamBook.ttf');
}

#app {
  font-family: spotify, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
