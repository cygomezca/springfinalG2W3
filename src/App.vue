<template>
  <div id="app">
    <header-item></header-item>
    <b-container fluid >
    <carousel-item></carousel-item>
    </b-container>
    <!-- Layout  -->
    <layout>
      <template slot="products">
          <product-list></product-list>
      </template>
      <template slot="cart">
          <cart></cart>
      </template>
    </layout>
    <!-- Layout - end -->
    <header-footer></header-footer>
  </div>
</template>

<script>
import Layout from '@/layouts/Layout'
import ProductList from '@/components/ProductsList'
import Cart from '@/components/Cart'
import CarouselItem from '@/components/CarouselItem'
import HeaderItem from './components/HeaderItem'
import HeaderFooter from './components/HeaderFooter.vue'



export default {
  name: 'App',
  components: {
    Layout, ProductList, Cart, CarouselItem, HeaderFooter, HeaderItem
  }
}
</script>

