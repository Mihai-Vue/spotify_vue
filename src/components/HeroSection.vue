<template>
  <section class="hero-section">
    <div class="content-wrapper">
      <h1>Ia-ți versiunea Premium gratuită timp de o lună</h1>
      <h2>Doar 4.99 EUR/lună după. Anulezi oricând.</h2>
      <button class="btn-1 buttons">SA INCEPEM</button>
      <button class="btn-2 buttons">VEZI ABONAMENTE</button>

      <p>
        <a class="a-hero">Se aplică Termeni și condiții.
        </a> Luna gratuită nu este disponibilă utilizatorilor care au încercat deja versiunea Premium.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "HeroSection.vue",

}
</script>

<style>
  .hero-section {
    background-color: #1d75de;
    height: 480px;
  }

  .content-wrapper {
    height: 305px;
    width: 1170px;
    padding: 72px 0;
    margin: 0 347px;
    text-align: start;
    color: white;
  }

  .content-wrapper h1 {
    .color: white;
    font-size: 40px;
    font-weight: bold;
    margin-top: 60px;
  }

  .content-wrapper h2 {
    margin-top: 30px;
  }

  .content-wrapper p {
    margin-top: 40px;
    font-size: 11px;
  }

  .a-hero {
    cursor: pointer;
    display: inline-block;
    text-decoration: underline;
  }

  .btn-1 {
    background-color: black;
    border: 2px solid black;
    margin-right: 8px;
  }

  .btn-2 {
    background-color: #1d75de;
    border: 2px solid white;
  }

  .buttons {
    color: white;
    font-weight: bold;
    padding: 14px 32px;
    border-radius: 25px;
    margin-top: 30px;
  }

</style>
