<template>
  <section class="subscription-section">
    <div class="subscription-wrapper">
      <h2 class="subscription-title">Alege-ți abonamentul Premium</h2>
      <h3>Asculți nelimitat pe telefon, în boxe și pe alte dispozitive.</h3>
      <SubscriptionCard />
    </div>
  </section>
</template>

<script>
import SubscriptionCard from './SubscriptionCard.vue';

export default {
  name: "SubscriptionSection.vue",
  components: {
    SubscriptionCard
  },

  data: () => {
      subscriptionList: [
        {
          nameOffer: "",
          priceDescription: "",
          acountNumber: "",
          offerDescription: 
            [
              "Ascultă muzică fără anunțuri", 
              "Redai de oriunde – chiar și offline", 
              "Redare la cerere"
            ],
          offerCondition: ""
        },
        {
          nameOffer: "",
          priceDescription: "",
          acountNumber: "",
          offerDescription: 
            [
              "2 conturi Premium pentru un cuplu care locuiește împreună", 
              "Asculți muzică fără reclame, redai offline și la cerere"
            ],
          offerCondition: ""
        },
        {
          nameOffer: "",
          priceDescription: "",
          acountNumber: "",
          offerDescription: 
            [
              "6 conturi Premium pentru membrii familiei care locuiesc împreună", 
              "Blochezi muzica având conținut explicit", 
              "Asculți muzică fără reclame, redai offline și la cerere"
            ],
          offerCondition: ""
        },
        {
          nameOffer: "",
          priceDescription: "",
          acountNumber: "",
          offerDescription: 
            [
              "Reducere specială pentru studenții eligibili care urmează cursurile unei universități", 
              "Ascultă muzică fără reclame", 
              "Redai de oriunde – chiar și offline",
              "Redare la cerere"
            ],
          offerCondition: ""
        },
      ]
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
}
</style>
