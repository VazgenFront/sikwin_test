<template>
  <vueper-slides
    :bullets="true"
    :arrows="false"
    :autoplay="true"
    fixed-height="380px"
    transition-speed="100"
    :touchable="false"
  >
    <vueper-slide v-for="(slide, i) in slides" :key="i" :image="slide.image" />
  </vueper-slides>
</template>

<script>
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";

export default {
  name: "slider-item",
  components: { VueperSlides, VueperSlide },

  data: () => ({
    slides: [
      { image: require("@/assets/slider-img1.jpg") },
      { image: require("@/assets/slider-img2.jpg") },
      { image: require("@/assets/slider-img3.jpg") },
      { image: require("@/assets/slider-img4.jpg") },
    ],
  }),
};
</script>

<style >
.thumbnails {
  margin: auto;
  max-width: 300px;
}

.thumbnails .vueperslide {
  box-sizing: border-box;
  border: 1px solid #fff;
  transition: 0.3s ease-in-out;
  opacity: 0.7;
  cursor: pointer;
}

.thumbnails .vueperslide--active {
  box-shadow: 0 0 6px rgba(0, 0, 0, 0.3);
  opacity: 1;
  border-color: #000;
}

.vueperslides__bullet .default  {
  width: 15px;
  height: 15px;
}
</style>
