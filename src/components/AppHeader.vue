<template>
  <div class="app-header">
    <img class="header-logo" src="../assets/spotify_logo.png" alt="spotify logo">
    <nav class="app-header-nav">
      <div class="nav-header" v-for="({route, name}, index) in navItems"
           :key="name">
        <a class="header-a" :href="route">
          {{name}}
        </a>
        <span id="pipe" v-if="index === 2">|</span>
      </div>
    </nav>
  </div>
</template>

<script>
  export default {
    name: "AppHeader.vue",
    data(){
      return {
        navItems: [
          {
            name: 'Premium',
            route: '#'
          },
          {
            name: 'Asistenta',
            route: '#'
          },
          {
            name: 'Descarca',
            route: '#'
          },
          {
            name: 'Inregistreaza-te',
            route: '#'
          },
          {
            name: 'Conecteaza-te',
            route: '#'
          }
        ]
      }
    }
  }
</script>

<style>

  .header-logo {
    height: 110px;
    cursor: pointer;
  }

  .app-header {
    background: black;
    display: flex;
    justify-content: space-around;
    height: 80px;
    align-items: center;
    padding: 0 160px;
  }

  .app-header-nav {
    color: black;
    display: flex;
    align-items: center;
    gap: 30px;
  }

  .nav-header {
   height: 8px;
  }

  .header-a {
    text-decoration: none;
    color: white;
    font-size: 14px;
    font-weight: bold;
    display: inline-block;
    padding: 8px 5px;
  }

  .header-a:hover {
    color: greenyellow;
    cursor: pointer;
  }

  #pipe {
    color: white;
    padding-left: 30px;
    font-size: 18px;
    font-weight: bold;
  }
</style>
