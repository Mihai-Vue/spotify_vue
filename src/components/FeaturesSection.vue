<template>
  <section class="feature-section">
    <div class="feature-wrapper">
      <h2 id="feature-title">De ce să treci la Premium?</h2>
      <ul>
        <li class="feature-list"
            v-for="{image, logo, featureOne, featureTwo} in featureList"
            :key="featureTwo"
            >
          <img class="feature-logo" :src= "image" :alt="logo">
          <p id="feature-one">{{featureOne}}</p>
          <p id="feature-two">{{featureTwo}}</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "FeaturesSection.vue",
  data:() => {
    return {
      featureList: [
        {
          image: require("../assets/music_download.png"),
          logo: "music download logo",
          featureOne: "Descarci muzică.",
          featureTwo: "Asculți de oriunde."
        },
        {
          image: require("../assets/music_no_adds.png"),
          logo: "music no adds logo",
          featureOne: "Ascultă muzică fără anunțuri.",
          featureTwo: "Te bucuri non-stop de muzică."
        },
        {
          image: require("../assets/play_any_song.png"),
          logo: "play any song logo",
          featureOne: "Redă orice melodie.",
          featureTwo: "Chiar și pe dispozitivul mobil."
        },
        {
          image: require("../assets/music.png"),
          logo: "music continuous play logo",
          featureOne: "Omiteri nelimitate.",
          featureTwo: "Doar apeși butonul Înainte."
        },
      ]
    }
  }
}
</script>

<style>

  .feature-section {
    background-color: white;
    color: #282828;
  }

  .feature-wrapper {
    height: 397px;
    width: 1140px;
    padding: 75px 15px;
    margin: 0 auto;
  }

  #feature-title{
    font-size: 35px;
    font-weight: bold !important;
    color: black;
  }

  .feature-wrapper ul {
    display: flex;
    justify-content:space-between;
    margin: 0;
    padding: 0;
  }

  ul {
    list-style-type: none;
  }

  .feature-logo {
    height: 150px;
    width: 150px;
  }

  #feature-one {
    font-size: 20px;
    font-weight: bold;
  }

  #feature-two {
    font-size: 16px;
  }

</style>
