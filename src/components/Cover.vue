<template>
    <v-container>
      <v-row justify="space-around">
        <v-card width="1200">
          <v-img
            height="150"
            src="https://cdn.pixabay.com/photo/2022/01/17/09/03/program-6944163_1280.jpg"
            cover
          ></v-img>

          
          <v-card-text class="centered-card-text">
              <h2 class="align-center centered-text my-4 pb-3 text-h4">Universidad Gerardo Barrios </h2>
            <v-timeline density="compact" align="start">
              <v-timeline-item
                v-for="subtitle in subtitles"
                :dot-color="subtitle.color"
                size="x-small"
              >
                <div class="mb-4">
                  <div class="font-weight-normal text-h6">
                    <strong>{{ subtitle.title }}</strong>
                  </div>
                  <div>{{ subtitle.subtitle }}</div>
                </div>
              </v-timeline-item>
            </v-timeline>
          </v-card-text>
        </v-card>
      </v-row>
    </v-container>
  </template>
  
  <style>
  .centered-card-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
  </style>
  
  <script>
  export default {
    data() {
      return {
        subtitles: [
          {
            title: 'Estudiante',
            subtitle: `Oscar Uvense Ayala Gonzáles`,
            color: 'blue',
          },
          {
            title: 'Docente',
            subtitle: 'MIW. Inga. Gisela Espinoza',
            color: 'blue',
          },
          {
            title: 'Asignatura',
            subtitle: 'Programación Computacional IV',
            color: 'blue',
          },
          {
            title: 'Nombre Actividad',
            subtitle: 'Portafolio de Cómputo 3',
            color: 'blue',
          },
          {
            title: 'Fecha de Entrega',
            subtitle: 'Domingo 11 de junio de 2023',
            color: 'blue',
          },
        ],
      };
    },
  };
  </script>
  