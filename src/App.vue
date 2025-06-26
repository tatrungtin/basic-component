<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <FirstComponent />
  <SecondComponent />
  <ProductList/>
  <hr>
  <br><br>
  <DemoSlots>
    <template v-slot:header>
      <h1>Header</h1>
    </template>
    <template v-slot:footer>
      <h1>Footer</h1>
    </template>
    <template v-slot:default>
      <h1>default</h1>
    </template>
  </DemoSlots>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import FirstComponent from './components/FirstComponent.vue';
import SecondComponent from './components/SecondComponent.vue';
import ProductList from './components/ProductList.vue';
import DemoSlots from './components/DemoSlots.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    FirstComponent,
    SecondComponent,
    ProductList,
    DemoSlots
  },
  provide(){
    return {
      user:"ta trung tin"
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
