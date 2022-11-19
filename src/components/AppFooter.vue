<template>
  <div class="app-footer">
    <img src="../assets/spotify_logo.png" alt="spotify logo">
      <nav>
        <div v-for="({name, items}) in footerNavItems" :key="name">
          <span>{{name}}</span>
          <a v-for="item in items"
             :href="item.route"
             :key="item.itemName">
            {{item.itemName}}
          </a>
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
      ]
    }
  }
}
</script>

<style scoped>
  .app-footer {
    background-color: black;
  }
</style>


COMPANIE
Despre
Locuri de muncă
For the Record
COMUNITĂȚI
Pentru Artiști
Dezvoltatori
Publicitate
Investitori
Furnizori
LINKURI UTILE
Asistență
Player web
Aplicație mobilă gratuită
