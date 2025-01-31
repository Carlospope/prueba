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
<!-- Carucel de imagenes -->
    <main>
        <section id="home">
            <div class="">
                <h2>Tortas</h2>
                <img :src="ima1" alt="" />
            </div>
            <p>Carnitas</p>
        </section>
    </main>

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
width: 100vh;
height: 100vh;
}
/* Menu principal */
.logo:hover  {
filter: drop-shadow(0 0 2em #ffffffaa);
}
.logo.vue:hover {
filter: drop-shadow(0 0 2em #42b883aa);
}
.contenedor{
background-color: #2ecc71;
width: 200px;
height: 200px;
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

header .logo h1 {
    margin-left: 100px;
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



</style>
