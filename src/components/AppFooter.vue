<template>
  <div class="app-footer">
    <img class="footer-logo" src="../assets/spotify_logo.png" alt="spotify logo">
    <nav class="footer-nav">
        <div class="footer-nav-div" v-for="({name, items}) in footerNavItems" :key="name">
          <span class="footer-span">{{name}}</span>
          <a class="footer-a" v-for="item in items"
             :href="item.route"
             :key="item.itemName">
            {{item.itemName}}
          </a>
        </div>
        <div class="social-link">
          <a href="#"><i class="fab fa-instagram"></i></a>
          <a href="#"><i class="fab fa-twitter"></i></a>
          <a href="#"><i class="fab fa-facebook-f" ></i></a>

        </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "AppFooter.vue",

  data(){
    return {
      footerNavItems: [
        {
          name: 'COMPANIE',
          items:[
            {
              itemName:'Despre',
              route:'#'
            },
            {
              itemName:'Locuri de muncă',
              route:'#'
            },
            {
              itemName:'For the record',
              route:'#'
            }
          ]
        },
        {
          name: 'COMUNITATI',
          items:[
            {
              itemName: 'Despre Artisti',
              route: '#'
            },
            {
              itemName:'Dezvoltatori',
              route: '#'
            },
            {
              itemName: 'Publicitate',
              route: '#'
            },
            {
              itemName: 'Investitori',
              route: '#'
            },
            {
              itemName: 'Furnizori',
              route: '#'
            },
          ]
        },
        {
          name: 'LINKURI UTILE',
          items:[
            {
              itemName:'Asistenta',
              route: '#'
            },
            {
              itemName:'Player web',
              route: '#'
            },
            {
              itemName:'Aplicatie mobila gratuita',
              route: ''
            }
          ]
        }
      ],
    }
  }
}
</script>

<style>
  .app-footer {
    background-color: black;
    display: flex;
    justify-content: center;
    margin-top: 30px;
    padding: 60px 0;
  }

  .footer-logo {
    height: 110px;
    cursor: pointer;
  }

  .footer-nav {
    display: flex;
  }

  .footer-span {
    color: #949292;
    font-size: 12px;
    font-weight: bold;
    display: block;
  }

  .footer-a {
    text-decoration: none;
    color: white;
    font-size: 14px;
    font-weight: bold;
    display: inline-block;
    padding: 8px 5px;
  }


  .footer-a:hover {
    .color: greenyellow;
  }

  .social-link {
    display: flex;
    gap: 45px;

  }

  .fa-facebook-f,
  .fa-instagram,
  .fa-twitter {
    font-size: 25px;
    color: white;
  }

  i:hover {
    color: greenyellow;
  }

  .footer-nav-div {
    display: flex;
    margin: 0 10px;
    flex-direction: column;
    align-items: start;
    gap: 25px;
  }
</style>


