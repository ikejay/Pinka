<template>
  <div id="app">
    <Header></Header>
    <Hero></Hero>
    <div class="row">
      <Product v-for="(prod, key) in prods" :key="key"></Product>
    </div>
  </div>
</template>

<script>


import Header from "@/components/Header/header";
import Hero from "@/components/Hero/hero";
import Product from "@/components/Product/product";

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Product
  },
  data() {
    return{
      prods: ['Cassava', 'Cocoa', 'Pigeon Pea', 'Watermelon', 'Cowpea']
    }
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.row {
  width: 100%;
  display: inline-flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
