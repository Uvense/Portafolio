<template>
  <v-card color="basil">
    <v-card-title class="text-center py-6">
      <h1 class="font-weight-bold text-h3 text-basil">
        Evaluaciones
      </h1>
    </v-card-title>

    <v-tabs v-model="tab" bg-color="transparent" color="blue" grow>
      <v-tab v-for="(item, index) in items" :key="index" :value="item">
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-window v-model="tab">
      <v-window-item v-for="(item, index) in items" :key="index" :value="item">
        <v-card color="basil" flat>
          <v-card-text>
            <div class="carousel-container">
              <!-- computo 1 -->
              <template v-if="index === 0">
                <v-card width="1000">
                  <v-carousel height="450">
                    <v-carousel-item
                      src="src\assets\Laboratorio1.jpg"
                    ></v-carousel-item>
                    <v-carousel-item
                      src="src\assets\Laboratio1.jpg"
                    ></v-carousel-item>
                    <v-carousel-item
                      src="src\assets\lab2.png"
                    ></v-carousel-item>
                  </v-carousel>
                </v-card>
              </template>
              <!-- computo 2 -->
              <template v-else-if="index === 1">
                <v-card width="1000">
                  <v-carousel height="450">
                    <v-carousel-item
                      src="src\assets\Lab1C2.png"
                    ></v-carousel-item>
                    <v-carousel-item
                      src="src\assets\Lab2C2.png"
                    ></v-carousel-item>
                  </v-carousel>
                </v-card>
              </template>
              <!-- computo 3 -->
              <template v-else-if="index === 2">
                <v-card width="1000">
                  <v-carousel height="450">
                    <v-carousel-item
                      src="src\assets\papeleta Lab 1.png"
                    ></v-carousel-item>

                    <v-carousel-item
                      src="src\assets\papeleta Lab 2.png"
                    ></v-carousel-item>
                  </v-carousel>
                </v-card>
              </template>
            </div>
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
  background-color: #ffffff !important;
}
.text-basil {
  color: #1b6fb3 !important;
}

.carousel-container {
  display: flex;
  justify-content: center;
}
</style>
