<template>
  <div id="app">
    <AppHeader />
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>Hello</h1>

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
