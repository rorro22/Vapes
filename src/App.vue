<template>
  <v-app>
    <v-container>
      <HelloWorld></HelloWorld>
      <Carrousel></Carrousel>
    </v-container>
    <Pie></Pie>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Carrousel from './components/Carrousel.vue'
import Pie from './components/Pie.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Carrousel,
    Pie
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Open+Sans');

body{
  display:flex;
  background-color:#F0F8FF;
  height:95vh;
  justify-content:center;
  align-items:flex-end;
  font-family:Open Sans;
}

#container{
  padding-top:20px;
  margin-top:20px;
  width:100vw;
  color:white;
  background-color:#292354;
  display:flex;
  flex-direction:column;
  align-items:center;
}


</style>
