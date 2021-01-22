<template>
  <div id="app">
    <img src="./assets/logo.png">
    <my-test/>
    <!--<router-view/>-->
    <color-block-1 bgColor1='Wheat'/>
    <ColorBlock v-bind:bgColor='Cls'/>
  </div>
</template>

<script>
import myTest from './components/myTest.vue'
import ColorBlock from './components/ColorBlock.vue'
import ColorBlock1 from './components/ColorBlock1.vue'
export default {
  components: { myTest, ColorBlock, ColorBlock1 },
  name: 'App',
  data () {
      return {
        Cls: [
          {color: 'OrangeRed'},
          {color: 'PaleGreen'},
          {color: 'RoyalBlue'},
          {color: 'SkyBlue'},
          {color: 'Tomato'},
          {color: 'Wheat'},
          {color: 'YellowGreen'},
          {color: 'Salmon'}]
      }
  } 
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
