<template>
  <section class="section-footer">
    <div class="app-footer">
        <div class="main-footer">
          <div class="footer-logo" >
            <img src="../assets/spotify_logo.jpg" alt="spotify logo">
          </div>
          <nav class="footer-nav">
              <div class="footer-nav-div" v-for="({ name, items }) in footerNavItems" :key="name">
                <span class="footer-span">{{ name }}</span>
                <a class="footer-a" v-for="item in items"
                   :href="item.route"
                   :key="item.itemName">
                  {{ item.itemName }}
                </a>
              </div>
          </nav>
          <div class="social-link">
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-facebook-f" ></i></a>
          </div>
        </div>
        <div class="ro-lang">
          <i class="fas fa-globe-europe"></i>
          <a>Romana(romana)</a>
        </div>
        <div class="footer-info">
          <ul class="footer-ul">
            <li class="footer-li"
                v-for="{ route, name } in footerInfoItems"
                :key="name">
              <a class="footer-link"
                  :href="route">
                {{ name }}
              </a>
            </li>
          </ul>
          <span class="footer-copyright">© 2022 Spotify AB</span>
        </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppFooter.vue",

  data: () => {
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
      footerInfoItems:[
        {
          name: "Legal (Informații juridice)",
          route: "#"
        },
        {
          name: "Centru de confidențialitate",
          route: "#"
        },
        {
          name: "Politică de confidențialitate",
          route: "#"
        },
        {
          name: "Setări pentru cookie-uri",
          route: "#"
        },
        {
          name: "About Ads (Informații despre reclame)",
          route: "#"
        },
      ]
    }
  }
}
</script>

<style>
  .section-footer {
    background-color: black;
    height: 500px;
  }

  .app-footer {
    margin: 0 367px;
    width: 1147px;
    height: 400px;
  }

  .footer-nav-div {
    padding: 0 15px;
    min-height: 346px;
    width: 195px;
  }

  .footer-logo {
    padding: 0 15px;
    height: 346px;
    width: 195px;
  }

  .footer-logo img {
    height: 110px;
    width: 165px;
    cursor: pointer;
  }

  .main-footer {
    display: flex;
  }

  .footer-nav {
    display: flex;
    padding-top: 20px;
  }

  .footer-span {
    color: #afadad;
    font-size: 12px;
    font-weight: bold;
    display: block;
    margin: 20px 0;
  }

  .footer-a {
    color: white;
    text-align: start;
    font-size: 16px;
    font-weight: bold;
    text-decoration: none;
    line-height: 1.3;
  }

  .footer-a:hover {
    color: greenyellow;
  }

  .social-link {
    margin: 0 15px 0 143px;
    width: 195px;
    height: 346px;
    display: flex;
    justify-content: space-between;
  }

  .fa-facebook-f,
  .fa-instagram,
  .fa-twitter {
    font-size: 25px;
    color: white;
    padding: 30px 0;
  }

  i:hover {
    color: greenyellow;
  }

  .footer-nav-div {
    display: flex;
    flex-direction: column;
    align-items: start;
    gap: 25px;
  }

  .ro-lang {
    color: #afadad;
    margin: 0 auto;
    text-align: end;
    cursor: pointer;
  }

  .footer-ul {
    display: inline-flex;
  }

  .footer-li {
    padding-right: 25px;
  }

  .footer-li:hover {
    color: greenyellow;
  }

  .footer-link {
    text-decoration: none;
    font-size: 11px;
    color: #afadad;
    display: block;
  }

  .footer-link:hover {
    color: greenyellow;
  }

  .footer-copyright {
    font-size: 12px;
    color: #afadad;
    padding-left: 100px;
  }

  .ro-lang:hover {
    color: greenyellow;
  }

</style>


