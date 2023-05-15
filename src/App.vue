<script setup>
import AppBar from './components/AppBar.vue'
import Gallery from './components/Gallery.vue'
import Schedule from './components/Schedule.vue'
import AboutMe from './components/AboutMe.vue'
import Intro from './components/Intro.vue'
</script>

<template>
  <div>
    <v-layout>
      <AppBar />
      <v-main>
        <v-container fluid class="pa-0">
          <Intro />
          <Gallery />
          <AboutMe />
          <Schedule />
        </v-container>
      </v-main>
    </v-layout>
  </div>
</template>

<style scoped></style>
