<template>
  <div id="app">
    <product-list-one :products="products" />
    <product-list-two :products="products" />
  </div>
</template>

<script>
//import { createStore } from 'vuex'
import ProductListOne from './components/ProductListOne.vue';
import ProductListTwo from './components/ProductListTwo.vue';

export default {
  name: 'app',
  components: {
    "product-list-one": ProductListOne,
    'product-list-two': ProductListTwo
  },
  data() {
    return {
      products: [
        { "name": "Banana Skin", price: 20 },
        { "name": "BSkinny Stars", price: 40 },
        { "name": "Green Shells", price: 60 },
        { "name": "Red Shells", price: 80 }

      ]
    }
  }
}
</script>

<style></style>
