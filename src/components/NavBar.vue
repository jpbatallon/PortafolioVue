<script setup></script>

<template>
  <body>
    <nav class="navMenu">
      <a href="#about">Sobre mi</a>
      <a href="#educacion">Educación</a>
      <a href="#proyectos">Proyectos</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </body>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap");
/* * {
  margin: 0;
  padding: 0;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
} */

body {
  /* background: #272727; */
  font-family: "Montserrat", sans-serif;
  margin-bottom: 0;
}

.navMenu {
  display: flex;
  position: relative;
  justify-content: center;
  margin-top: 50px;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}

.navMenu a {
  color: #f6f4e6;
  text-decoration: none;
  font-size: 1.2em;
  text-transform: uppercase;
  font-weight: 500;
  display: inline-block;
  width: auto;
  padding: 30px;
  -webkit-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
}

.navMenu a:hover {
  color: #36a8fa;
}
</style>
