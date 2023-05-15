<script>
export default {
  data() {
    return {
      title: 'Groovy',
      colors: ['indigo', 'warning', 'pink darken-2', 'red lighten-1', 'deep-purple accent-4'],
      slides: ['First', 'Second', 'Third', 'Fourth', 'Fifth']
    }
  }
}
</script>
<template>
  <div id="gallery" class="main">
    <h1>GALLERY</h1>
    <v-carousel cycle height="400" width="90" hide-delimiter-background show-arrows="hover">
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-sheet :color="colors[i]" height="100%">
          <div class="d-flex fill-height justify-center align-center">
            <div class="text-h2">{{ slide }} Slide</div>
          </div>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
  </div>
</template>
<style>
.main {
  width: 100vw;
  height: 100vh;
  text-align: center;
}
.main h1 {
  padding-right: 50%;
  padding-top: 10px;
  margin-bottom: 15px;
}
</style>
