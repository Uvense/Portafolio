<template>
  <v-card color="basil">
    <v-card-title class="text-center py-6">
      <h1 class="font-weight-bold text-h3 text-basil">
        Contenidos
      </h1>
    </v-card-title>

    <v-tabs
      v-model="tab"
      bg-color="transparent"
      color="blue"
      grow
    >
      <v-tab
        v-for="(item, index) in items"
        :key="index"
        :value="item"
      >
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-window v-model="tab">
      <v-window-item
        v-for="(item, index) in items"
        :key="index"
        :value="item"
      >
        <v-card
          color="basil"
          flat
        >
          <v-card-text class="text-center">
            <template v-if="index === 0">
              <b>Desarrollo Frontend con librerías del lado del cliente</b> <br/>
              <div>
                  Introducción a JavaScript Básico <br/>
                  Introducción a las librerías (Vue.js y Bootstrap)<br/>
                  Rendering declarativo y manipulación del DOM<br/>
                  Introducción al rendenring declarativo<br/>
                  Expresiones, propiedades y control de flujos con directivas<br/>
                  Renderizado de listas<br/>
                  Manejo de eventos Clases y estilos en tiempo real<br/>
                  Sistema de componentes<br/>
                  Crear componentes Custom<br/>
                  Comunicación entre componentes: propiedades y eventos<br/>
              </div>
            </template>
            <template v-else-if="index === 1">
              <b>Desarrollo Backend con el Framework del lado del servidor y base de datos</b>
              <div>
                  Introducción al desarrollo con PHP<br/>
                  Declaración de variables<br/>
                  Declaración de funciones<br/>
                  Programación orientada a objetos<br/>
                  Conexión a base de datos<br/>
                  Introducción a Laravel<br/>
                  CRUD con Laravel<br/>
              </div>
            </template>
            <template v-else-if="index === 2">
              <strong>Incorporando tecnologías de Servidor Web</strong>
              <div>
                  Formularios Laravel<br/>
                  Sistema de rutas y controladores<br/>
                  Validación de datos<br/>
                  Blade: sistema de plantillas avanzado<br/>
                  Trabajando con Laravel/UI<br/>
                  Creación de API REST con Laravel<br/>
                  Consumo de API REST<br/>
              </div>
            </template>
          </v-card-text>
        </v-card>
      </v-window-item>
    </v-window>
  </v-card>
</template>

<script setup>
  import { ref } from 'vue'

  const tab = ref('Cómputo 1')

  const items = [
    'Cómputo 1',
    'Cómputo 2',
    'Cómputo 3',
  ]
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
