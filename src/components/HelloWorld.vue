<template>
  <div class="header">
    <img src="@/assets/logo.png" alt="Logo" class="logo">
    <h1>Rodri me la pela</h1>
    <!-- Agrega más contenido según sea necesario -->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
};
</script>

<style>
.header {
  grid-area: 1 / 1 / 2 / 4;
}

.logo {
  width: 50px;
  margin-right: 15px;
}
</style>
