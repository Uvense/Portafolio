<template>
    <v-card color="basil">
        <v-card-title class="text-center justify-center py-6">
        <h1 class="font-weight-bold text-h3 text-basil">
            Introducción
        </h1>
        </v-card-title>
        <div class="text-center text-h6">
            Bienvenidos a mi portafolio en línea, en el cual compartiré los conocimientos y habilidades adquiridos en el primer <br>
            cómputo de la asignatura de Programación Computacional IV. <br>
            Durante este cómputo, hemos aprendido los fundamentos de Vue, un framework progresivo de JavaScript utilizado para <br>
            construir interfaces de usuario. Entre los temas que se han abordado se encuentran: la creación de componentes, la gestión <br>
            de datos y eventos, el enrutamiento, el uso de Directivas, el ciclo de vida de los componentes, entre otras cosas.<br>
            <br>
            Para demostrar mi comprensión y aplicación de estos temas, presentaré evidencias de guías resueltas, tareas y proyectos, <br>
            así como investigaciones y exámenes. Espero poder aplicar estos conocimientos en futuros proyectos.<br>
            <br>
            A través de mi portafolio en línea, espero demostrar mi compromiso con el aprendizaje continuo. <br>
            ¡Gracias por visitar mi portafolio en línea!
        </div>
    </v-card>
  </template>
  
  <script setup>
    import { ref } from 'vue'
    const title = ref('Introducción')

  </script>
  
  <style>
  /* Helper classes */
  .bg-basil {
    background-color: #e6fffe !important;
  }
  .text-basil {
    color: #1b6fb3 !important;
  }
  </style>
  