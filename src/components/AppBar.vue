<script>
export default {
  data() {
    return {
      title: 'Groovy'
    }
  }
}
</script>
<template>
  <v-app-bar color="transparent" class="elevation-0 text-white" fixed>
    <v-app-bar-title class="text-h5" href="#home">{{ title }}</v-app-bar-title>

    <template v-slot:append>
      <v-btn href="#gallery">Gallery</v-btn>
      <v-btn href="#about">The Hair Artist</v-btn>
      <v-btn href="#schedule">Book Now!</v-btn>
    </template>
  </v-app-bar>
</template>
