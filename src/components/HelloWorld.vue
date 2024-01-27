<template>
  <div class="header">
      <div class="left-section">
        <img src="@/imagenes/logito.jpg" alt="Logo" class="logo"> 
        <h1>Bodeguita Vapes</h1>
      </div>
      <div class="right-section">
        <nav class="navbar">
          <router-link to="/">Inicio</router-link>
          <router-link to="/productos">Productos</router-link>
          <router-link to="/contacto">Contacto</router-link>
          <!-- Agrega más enlaces del navbar según sea necesario -->
        </nav>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
};
</script>

<style scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #000000;
  color: #fff;
  padding: 15px;
  display: flex;
  justify-content: space-between; /* Centra el contenido horizontalmente */
}

.center-section {
  display: flex;
  align-items: center;
  width: 100%;
  max-width: 1200px; /* Ajusta según sea necesario */
}

.left-section {
  display: flex;
  align-items: center;
}

.left-section img {
  width: 14%;
}

.logo {
  width: 50px;
  margin-right: 15px;
}

.right-section {
  display: flex;
  align-items: center;
  margin-right: 10%;
}

.navbar {
  display: flex;
  position: relative;
}

.navbar router-link {
  margin-right: 10%;
  font-size: larger;
  text-decoration: none;
  color: #fff;
  font-weight: bold;
  transition: color 0.3s ease;
}

.navbar router-link:hover {
  color: #ffcc00;
}

</style>
