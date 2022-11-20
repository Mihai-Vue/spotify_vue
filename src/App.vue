<template>
  <div id="app">
    <AppHeader />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader";
import AppFooter from "@/components/AppFooter";

export default {
  name: 'App',
  components: {
      AppHeader,
      AppFooter,
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



/*
https://www.spotify.com/ro-ro/premium/?utm_source=ro-en_brand_contextual-desktop_text&utm_medium=paidsearch&utm_campaign=alwayson_emea_ro_performancemarketing_core_brand+contextual-desktop+text+bmm+ro-en+google&gclid=Cj0KCQiA37KbBhDgARIsAIzce16n2dOM-RBfzhBypUm-tef1A0cC880L7m6YTsFxRw7MpAavYX6_kUUaAgHrEALw_wcB&gclsrc=aw.ds
*/
