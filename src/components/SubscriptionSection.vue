<template>
  <section class="subscription-section">
    <div class="subscription-wrapper">
      <h2 class="subscription-title">Alege-ți abonamentul Premium</h2>
      <h3>Asculți nelimitat pe telefon, în boxe și pe alte dispozitive.</h3>
      <SubscriptionCard class="subscription"
        v-for="item in list" 
        :key="item.id"
        :name-offer="item.nameOffer"
        :price-description="item.priceDescription"
        :account-number="item.accountNumber"
        :offer-description="item.offerCondition"
        :offer-condition="item.offerCondition"
      />
    
    </div>
  </section>
</template>

<script>
import SubscriptionCard from './SubscriptionCard.vue';

export default {
  name: 'SubscriptionSection',
  components: {
    SubscriptionCard,
  },

  data:() => {
    return {
      list: [
        {
          id: "1",
          nameOffer: "Individual",
          priceDescription: "4.99 EUR/lună după perioada ofertei",
          accountNumber: "Un cont",
          offerDescription:
            [
              "Ascultă muzică fără anunțuri", 
              "Redai de oriunde – chiar și offline", 
              "Redare la cerere"
            ],
          offerCondition: 
            `
              Se aplică Termeni și condiții.
              Luna gratuită nu este disponibilă utilizatorilor
              care au încercat deja versiunea Premium.
            `
        },
        {
          id: "2",
          nameOffer: "Duo",
          priceDescription: "6.49 EUR/lună după perioada ofertei",
          acountNumber: "2 conturi",
          offerDescription: 
            [
              "2 conturi Premium pentru un cuplu care locuiește împreună", 
              "Asculți muzică fără reclame, redai offline și la cerere"
            ],
          offerCondition: 
              `
                Se aplică Termeni și condiții.
                Luna gratuită nu este disponibilă utilizatorilor
                care au încercat deja versiunea Premium.
              `
        },
        {
          id: "3",
          nameOffer: "Familie",
          priceDescription: "7.99 EUR/lună după perioada ofertei",
          acountNumber: "Maximum 6 conturi",
          offerDescription: 
            [
              "6 conturi Premium pentru membrii familiei care locuiesc împreună", 
              "Blochezi muzica având conținut explicit", 
              "Asculți muzică fără reclame, redai offline și la cerere"
            ],
          offerCondition: 
            `
              Se aplică Termeni și condiții.
              Luna gratuită nu este disponibilă utilizatorilor
              care au încercat deja versiunea Premium.
            `
        },
        {
          id: "4",
          nameOffer: "Student",
          priceDescription: "2.49 EUR/lună după perioada ofertei",
          acountNumber: "Un cont",
          offerDescription: 
            [
              "Reducere specială pentru studenții eligibili care urmează cursurile unei universități", 
              "Ascultă muzică fără reclame", 
              "Redai de oriunde - chiar și offline",
              "Redare la cerere"
            ],
          offerCondition: ""
        },
      ]
    }  
  }
}
</script>
  export default {
    data: () => {
      return {
      }
    }
  }
<style>

.subscription-section {
  background-color: #EFEFEF;
  height: 927px;
  margin: 0;
  display: flex;
  justify-content:space-between;

}

.subscription-wrapper {
  
}

</style>
