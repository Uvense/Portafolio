<template>
  <v-card-title class="text-center py-6">
    <h1 class="font-weight-bold text-h3 text-basil">
      Investigaciones
    </h1>
  </v-card-title>
    <v-container>
      <v-row justify="space-around">
        <v-card width="450">
          <v-img
            height="200"
            src="https://cdn.pixabay.com/photo/2016/09/13/11/04/browser-1666982_1280.png"
            cover
          ></v-img>
        </v-card>
      </v-row>
    </v-container>
    <div class="text-center text-h5">
      <br>
      Cómputo 3
      <ul>
        <li>
          <a href="https://www.youtube.com/watch?v=j5baJsM_Adc" target="_blank">Investigación 1</a>
        </li>
        <br>
        <li>
          <a href="https://www.youtube.com/watch?v=aYfRTdaEY3s&t" target="_blank">Investigación 2</a>
        </li>
      </ul>
      <br>
  </div>
  </template>
  
  <script>
  export default {
    data: () => ({
        tab: null
    })
  };
  </script>