<template>
  <div class="app-header">
    <img src="../assets/spotify_logo.jpg" alt="spotify logo">
    <nav>
      <a v-for="item in navItems">{{item.name}}</a>
    </nav>
    <a></a>
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
    width: 200px;
  }

  .app-header {
    background: black;
    display: flex;
    justify-content: space-around;
  }

  nav {
    color: white;
    display: flex;
    align-items: center;
  }

  a {
    padding-right: 20px;
  }
</style>
