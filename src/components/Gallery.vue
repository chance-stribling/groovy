<script>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/vue-splide/css';

document.addEventListener( 'DOMContentLoaded', function () {
  new Splide( '#thumbnail-carousel', {
		fixedWidth : 100,
    fixedHeight: 60,
		gap        : 10,
		rewind     : true,
		pagination : false,
  } ).mount();
} );

export default {
  components: {
    Splide,
    SplideSlide,
  },
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
    <div style="width: 50vw; height: 50vh;" class="mx-auto">
      <section
  id="thumbnail-carousel"
  class="splide"
  aria-label="The carousel with thumbnails. Selecting a thumbnail will change the Beautiful Gallery carousel."
>
  <div class="splide__track">
		<ul class="splide__list">
			<li class="splide__slide">
				<img src="../assets/tup.jpg" alt="">
			</li>
			<li class="splide__slide">
				<img src="../assets/hairflip.jpg" alt="">
			</li>
			<li class="splide__slide">
				<img src="../assets/tup.jpg" alt="">
			</li>
		</ul>
  </div>
</section>
    </div>
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
.splide__slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
