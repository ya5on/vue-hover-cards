<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h2>Hover over the cards</h2>
    <div class="container">
      <card data-image="https://images.unsplash.com/photo-1479660656269-197ebb83b540?dpr=2&auto=compress,format&fit=crop&w=1199&h=798&q=80&cs=tinysrgb&crop=">
        <h1 slot="header">Canyons</h1>
        <p slot="content">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
      </card>
      <card data-image="https://images.unsplash.com/photo-1479659929431-4342107adfc1?dpr=2&auto=compress,format&fit=crop&w=1199&h=799&q=80&cs=tinysrgb&crop=">
        <h1 slot="header">Beaches</h1>
        <p slot="content">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
      </card>
      <card data-image="https://images.unsplash.com/photo-1479644025832-60dabb8be2a1?dpr=2&auto=compress,format&fit=crop&w=1199&h=799&q=80&cs=tinysrgb&crop=">
        <h1 slot="header">Trees</h1>
        <p slot="content">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
      </card>
      <card data-image="https://images.unsplash.com/photo-1479621051492-5a6f9bd9e51a?dpr=2&auto=compress,format&fit=crop&w=1199&h=811&q=80&cs=tinysrgb&crop=">
        <h1 slot="header">Lakes</h1>
        <p slot="content">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
      </card>
    </div>
  </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'app',
  components: {
    Card
  }
}
</script>

<style lang="scss">
  body {
    margin: 40px 0;
    font-size: 14px;
    font-weight: 500;
    background-color: #BCAAA4;
    -webkit-font-smoothing: antialiased;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  .container {
    padding: 40px 80px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  h1 {
    font-size: 34px;
    font-weight: 700;
    color: #fff;
    text-align: center;
  }
  h2 {
    font-size: 24px;
    font-weight: 700;
    color: #5D4037;
    text-align: center;
  }
</style>
