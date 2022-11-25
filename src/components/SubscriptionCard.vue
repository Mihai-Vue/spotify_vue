<template>
  <div class="subscription-card">
    <div class="subscription-header">
      <span>O luna gratuit</span>
      <h3 class="subscription-title">{{}}</h3>
      <p>{{}}</p>
      <p>{{}}</p>
    </div>
    <ul>
      <li><img src="#" alt="#">{{}}</li>
    </ul>
    <button type="button" class="btn">SA INCEPEM</button>
    <p>{{}}</p>
  </div>
</template>

<script>
  export default {
    name: "SubscriptionCard.vue",
    props: {
      nameOffer, 
      priceDescription,
      acountNumber,
      offerDescription,
      offerCondition
    },
    data: () => {
        return {

        }
      }
  }
</script>

<style>
  .subscription-header {
    background-color: red;
  }


  .subscription-header > span {
    background-color: #1d75de;
    color: white;
    font-weight: bold;
    padding: 4px 8px;
    border-radius: 5px;
  }


</style>