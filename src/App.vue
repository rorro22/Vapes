<template>
  <div class="layout">
      <HelloWorld></HelloWorld>
      <Carrousel></Carrousel>
      <Promociones></Promociones>
      <Catalogo></Catalogo>
      <Carrito></Carrito>
      <Pie></Pie>
    </div>
</template>

<script>
import Promociones from "@/components/CatalogoTienda/Promociones.vue";
import Carrito from "@/components/CatalogoTienda/Carrito.vue";
import Catalogo from "@/components/CatalogoTienda/Catalogo.vue";
import HelloWorld from '@/components/HelloWorld.vue'
import Carrousel from '@/components/Carrousel.vue'
import Pie from '@/components/Pie.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Promociones,
    Carrito,
    Catalogo,
    Carrousel,
    Pie
  }
}

</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Open+Sans');

body{
  background-color:#F0F8FF;
  font-family:Open Sans;
}

.layout {
  display: grid;
  grid-template-columns: 3fr 2fr 3fr;
  grid-template-rows: minmax(10vh, auto) minmax(40vh, auto) 4fr 1fr;
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

.header {
  grid-area: 1 / 1 / 2 / 3;
}

.seccion {
  background-color: blueviolet;
  height: inherit;
}

.Catalogo {
  grid-area: 3 / 3 / -1 / 4;
}
.Promociones {
  grid-area: 3 / 1 / -1 / 2;
}

.Carrito {
  grid-area: 3 / 2 / -1 / 3;

}

  @media (max-width: 1200px) {

  .layout {
    grid-template-columns: 1fr  2fr;
    grid-template-rows: minmax(10vh, auto) minmax(40vh, auto) 4fr 1fr;
  }
  
  .header {
    grid-area: 1 / 1 / 2 / 2;
  }

  .Carrito {
     display: none;
  }
  
  .Catalogo {
    grid-area: 3 / 2 / 4 / 3;
  }
  
  .Promociones {
      grid-area: 3 / 1 / 4 / 2;
    }
  }
</style>
