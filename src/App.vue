<template>
  <div class="layout">
      <HelloWorld></HelloWorld>
      <div class="layoutCatalogoTienda">
        <Promociones></Promociones>
        <Carrito></Carrito>
        <Catalogo></Catalogo>
      </div>
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
    grid-template-rows: 1fr 4fr 4fr 1fr;
  }

  .layoutCatalogoTienda {
    color: black;
    grid-area: 3 / 1 / 4 / 4;
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    align-items: flex-start;
  }

  .seccion {
    background-color: blueviolet;
    height: inherit;
  }
</style>
