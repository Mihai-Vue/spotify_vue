<template>
  <div class="app-header">
    <img src="../assets/spotify_logo.png" alt="spotify logo">
    <nav>
      <a class="link" v-for="({route, name}, index) in navItems"
         :href="route"
         key="name">
        {{name}}
        <span v-if="index === 2">|</span>
      </a>
    </nav>
  </div>
</template>

<script>
  export default {
    data(){
      return {
        navItems: [
          {
            name: 'Premium',
            route: '#'
          },
          {
            name: 'Support',
            route: '#'
          },
          {
            name: 'Download',
            route: '#'
          },
          {
            name: 'Sign up',
            route: '#'
          },
          {
            name: 'Log in',
            route: '#'
          }
        ]
      }
    }
  }
</script>

<style>

  div img {
    height: 110px;
    cursor: pointer;
  }

  .app-header {
    background: black;
    display: flex;
    justify-content: space-around;
    height: 80px;
    align-items: center;
  }

  nav {
    color: white;
    display: flex;
    align-items: center;
  }

  .link {
    padding-right: 35px;
    text-decoration: none;
    color: white;
    cursor: pointer;
  }

  .link:hover {
    color: greenyellow;
  }

  span {
    margin-left: 30px;
  }
</style>
