<template>
    <v-card>
      <v-tabs
        v-model="tab"
        bg-color="primary"
      >
        <v-tab value="one">Inicio</v-tab>
        <v-tab value="two">Acerca de</v-tab>
        <v-tab value="three">Sumario de Contenidos</v-tab>
        <v-tab value="four">Apuntes de Clase</v-tab>
        <v-tab value="five">Guías de Laboratorio</v-tab>
        <v-tab value="six">Casos de Estudio</v-tab>
        <v-tab value="seven">Investigaciones</v-tab>
        <v-tab value="eigth">Papeletas y evidencias de evaluaciones</v-tab>
        <!-- <v-tab value="nine">Proyecto Integrador</v-tab> -->
    </v-tabs>
  
      <v-card-text>
        <v-window v-model="tab">
          <v-window-item value="one">
            <cover></cover>
          </v-window-item>
  
          <v-window-item value="two">
            <about></about>
          </v-window-item>
        
          <v-window-item value="three">
            <contents></contents>
          </v-window-item>
          <v-window-item value="four">
            <notes></notes>
          </v-window-item>
          <v-window-item value="five">
            <lab-guides></lab-guides>
          </v-window-item>
          <v-window-item value="six">
            <case-studies></case-studies>
          </v-window-item>
          <v-window-item value="seven">
            <investigations></investigations>
          </v-window-item>
          <v-window-item value="eigth">
            <evaluations></evaluations>
          </v-window-item>
          <!-- <v-window-item value="nine">
            <project></project>
          </v-window-item> -->
        </v-window>
      </v-card-text>
    </v-card>
  </template>
  

<script>
    import About from './About.vue';
    import Cover from './Cover.vue';
    import Notes from './Notes.vue';
    import Contents from './Contents.vue';
    import LabGuides from './LabGuides.vue';
    import CaseStudies from './CaseStudies.vue';
    import Investigations from './Investigations.vue';
    import Evaluations from './Evaluations.vue';

    export default {
        components: {
            About,
            Cover,
            About,
            Notes,
            Contents,
            LabGuides,
            CaseStudies,
            Investigations,
            Evaluations
        },
        data: () => ({
            tab: null
        })
    }
</script>