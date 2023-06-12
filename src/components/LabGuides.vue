<template>
  <v-card color="basil">
    <v-card-title class="text-center py-6">
      <h1 class="font-weight-bold text-h3 text-basil">
        Guias de Laboratorio
      </h1>
    </v-card-title>
    <v-container>
      <v-row justify="space-around">
        <v-card width="150">
          <v-img
            height="150"
            src="https://cdn.pixabay.com/photo/2016/04/01/11/10/boy-1300226_1280.png"
            cover
          ></v-img>
        </v-card>
      </v-row>
    </v-container>
    <br>
    <div class="text-center text-h5">
      Cómputo 1
      <ul>
        <li>
          <a href="https://github.com/Uvense/PROGRA4/" target="_blank">Enlace 1 a GitHub</a>
        </li>
        <li>
          <a href="https://github.com/Uvense/PrograIV_OSCAR" target="_blank">Enlace 2 a GitHub</a>
        </li>
        <li>
          <a href="https://github.com/Uvense/Parcial-1" target="_blank">Parcial</a>
        </li>
      </ul>
  </div>
  <br>
  <div class="text-center text-h5">
    Cómputo 2
    <ul>
      <li>
        <a href="https://github.com/Uvense/Portafolio-" target="_blank">Portafolio</a>
      </li>
      <li>
        <a href="https://github.com/Uvense/Parcial_II" target="_blank">Parcial</a>
      </li>
    </ul>
  </div>
  <br>
  <div class="text-center text-h5">
    Cómputo 3
    <ul>
      <li>
        <a href="https://github.com/Uvense/laboratorioI" target="_blank">Enlace 1 a GitHub - Laboratorio 1</a>
      </li>
      <li>
        <a href="https://github.com/Uvense/laboratorioll" target="_blank">Enlace 2 a GitHub - Laboratorio 2</a>
      </li>
      <li>
        <a href="https://github.com/Uvense/Parcial3" target="_blank">Parcial 3</a>
      </li>
    </ul>
    <br>
  </div>
  </v-card>
</template>

<script>
export default {
  data: () => ({
      tab: null
  })
};
</script>

<style>
/* Helper classes */
.bg-basil {
  background-color: #ffffff !important;
}
.text-basil {
  color: #1b6fb3 !important;
}
</style>
