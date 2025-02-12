<script setup>
import HelloWorld from './components/HelloWorld.vue'
import ima1 from './assets/Imagenes/tacos.jpg';
import ima2 from './assets/Imagenes/torta.jpg';
</script>
<template>
<html lang="es">
<body>

    <!-- Encabezado -->
    <header>
        <div class="logo">
            <h1>TORTAS AHOGADAS EL POPE</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Menu</a></li>
                <li><a href="#about">Realizar pedido a domicílio </a></li>
            </ul>
        </nav>
    </header>
<!-- pedido -->
<div class="container">
    <h1>Formulario de Pedido</h1>
    <form action="#" method="POST">
    <div class="form-group">
        <label for="nombre">Nombre Completo:</label>
        <input type="text" id="nombre" name="nombre" required>
    </div>
    <div class="form-group">
        <label for="direccion">Dirección de Envío:</label>
        <input type="text" id="direccion" name="direccion" required>
    </div>
    <div class="form-group">
        <label for="producto">Producto:</label>
        <select id="producto" name="producto" required>
        <option value="camiseta">Tortas</option>
        <option value="pantalones">Tacos dorados</option>
        <option value="zapatos">Tacos blanditos </option>
        </select>
    </div>
    <div class="form-group">
        <label for="cantidad">Cantidad:</label>
        <input type="number" id="cantidad" name="cantidad" min="1" required>
    </div>
    <div class="form-group">
        <button type="submit">Realizar Pedido</button>
    </div>
    </form>
    </div> 
</body>
</html>
</template>
<style scoped>
.logo {
height: 6em;
padding: 1.5em;
will-change: filter;
transition: filter 300ms;
}
body{
    font-family: Arial, Helvetica, sans-serif;
}
/*Plasmado a todos */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
/* Estilos para el encabezado */
header {
    background-color: #333;
    color: #fff;
    padding: 20px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    top: 0;
    position: absolute;
    right: 0;
    left: 0;
}

nav ul {
    list-style: none;
    display: flex;
    margin-right: 20px;
}

nav ul li {
    margin: 0 30px;
}
nav ul li a {
    color: #ffffff;
    text-decoration: none;
    font-weight: bold;
}
/* Estilos para el contenido principal */
main {
    padding: 50px;
    margin-top: 50px;
}
section {
    margin-bottom: 80px;
}
h2 {
    color: #000000;
}
/* Estilos para el pie de página */
.logo{
background-color:rgb(155, 7, 7);
}
.carruselContenido{
    width: 100%;
    max-width: 600%;
    margin: auto;
    overflow: hidden;
}
.carruselItem{
    display: flex;
    transition: transform 0.5s ease
}
.carruselItem{
    min-width: 100%;
    display: flex;
    justify-content: center;
}
.carruselItem img{
    width: 100%;
    height: auto;
}
body {
font-family: Arial, sans-serif;
background-color: #ffffff;
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
}
/* Degradado del container */
.container {
background-color: rgb(255, 255, 255);
padding: 20px;
border-radius: 8px;
box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
width: 100%;
max-width: 500px;
}

h1 {
text-align: center;
margin-bottom: 20px;
}

/* Estilos para el formulario */
.form-group {
margin-bottom: 15px;
}

label {
display: block;
font-size: 14px;
color: #333;
margin-bottom: 5px;
}

input[type="text"], input[type="number"], select {
width: 100%;
padding: 10px;
border: 1px solid #ddd;
border-radius: 4px;
font-size: 16px;
}

button {
width: 100%;
padding: 10px;
background-color:rgb(155, 7, 7);
color: rgb(255, 255, 255);
border: none;
border-radius: 4px;
font-size: 16px;
cursor: pointer;
}
button:hover {
    background-color:rgb(62, 194, 10);
}
</style>
