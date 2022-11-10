<template>
  <div class="app-header">
    <img src="../assets/spotify_logo.png" alt="spotify logo">
    <nav>
      <a class="link" v-for="{url, name, index} in navItems" :href="url" key="name">{{name}}</a>
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
            url: '#'
          },
          {
            name: 'Support',
            url: '#'
          },
          {
            name: 'Download',
            url: '#'
          },
          {
            name: 'Sign up',
            url: '#'
          },
          {
            name: 'Log in',
            url: '#'
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
</style>
