<template>
  <div class="header">
    <img src="@/assets/logo.png" alt="Logo" class="logo">
    <h1>Bodeguita Vapes</h1>
    <!-- Agrega más contenido según sea necesario -->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
};
</script>

<style scoped>
.header {
  position: fixed; /* Establece la posición fija */
  top: 0; /* Fija el encabezado en la parte superior */
  left: 0;
  width: 100%; /* Ocupa todo el ancho de la pantalla */
  background-color: #333; /* Color de fondo oscuro */
  color: #fff; /* Color del texto */
  padding: 15px; /* Espaciado interno */
  display: flex; /* Utiliza un modelo de caja flexible para el diseño */
  align-items: center; /* Centra verticalmente los elementos en el contenedor */
}

.logo {
  width: 50px; /* Ajusta el ancho del logo según sea necesario */
  margin-right: 15px; /* Agrega espacio entre el logo y el texto */
}

/* Agrega estilos adicionales según sea necesario */
</style>
