<template>
  <div class="layout">
      <HelloWorld></HelloWorld>
      <Promociones></Promociones>
      <Catalogo></Catalogo>
      <Carrito></Carrito>
    </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Promociones from "@/components/CatalogoTienda/Promociones.vue";
import Carrito from "@/components/CatalogoTienda/Carrito.vue";
import Catalogo from "@/components/CatalogoTienda/Catalogo.vue";

export default {
  name: 'App',
  components: {
    HelloWorld,
    Promociones,
    Carrito,
    Catalogo
}
}
</script>

<style>
  .layout {
    display: grid;
    grid-template-columns: 3fr 2fr 3fr;
    grid-template-rows: minmax(10vh, auto) minmax(40vh, auto) 4fr 1fr;
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
