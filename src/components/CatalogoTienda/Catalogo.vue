<template>
  <div class="Catalogo">
    <h1>CatalogoTienda</h1>
    <div class="seccion contenido">
      <div v-for="index in 30" :key="index" class="producto">
        <img :src="'https://placekitten.com/200/300?image=' + index" alt="Gatito" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Catalogo',
}
</script>

<style scoped>
.contenido {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
}

/* Estilos opcionales para cada imagen de gatito */
.producto {
  margin: 10px;
  /* Otros estilos según sea necesario */
}
</style>