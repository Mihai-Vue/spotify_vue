<template>
  <div class="subscription-card">
    <div class="subscription-header">
      <span>O luna gratuit</span>
      <h3 class="subscription-title">{{ nameOffer }}</h3>
      <p>{{ priceDescription }}</p>
      <p>{{ accountNumber }}</p>
    </div>
    <ul>
      <li><img src="#" alt="#">{{}}</li>
    </ul>
    <button type="button" class="btn">SA INCEPEM</button>
    <p>{{offerCondition}}</p>
  </div>
</template>

<script>
  export default {
    name: 'SubscriptionCard',
    props: [
      'nameOffer', 
      'priceDescription',
      'accountNumber',
      'offerDescription',
      'offerCondition'
    ],
    data: () => {
        return {

        }
      }
  }
</script>

<style>
  .subscription-header {
    
  }


  .subscription-header > span {
    background-color: #1d75de;
    color: white;
    font-weight: bold;
    padding: 4px 8px;
    border-radius: 5px;
  }

  .subscription-card {
    display: inline-flex;
    flex-direction: column;
    width: 15%;
    height: 55%;
    margin: 0 10px;
    border: 1px solid black;
    border-radius: 8px;
    background-color:white;
  }
</style>
