<template>
    <div class="collection">
        <h1>Collection:</h1>
    </div>
  
    <ProductsVue/>
  </template>
  
  <script>
  import ProductsVue from '../components/Products.vue'
  // import SpinnerVue from '../components/Spinner.vue'
  
  export default {
  name: 'Products',
  components: {
    ProductsVue,
    // SpinnerVue
  }
  }
  </script>
  
  
  <style scoped>
  
  </style>