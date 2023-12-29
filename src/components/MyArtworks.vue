<script setup>
const artworks = [
  'artwork_1.png',
  'artwork-2.png',
  'artwork-3.png',
  'artwork-4.png',
  'artwork-5.png',
  'artwork-6.png'
]
import { ref } from 'vue'

let isIntersecting = ref(false)

const onIntersect = (isInter, entries, observer) => {
  isIntersecting.value = isInter
}
</script>

<template>
  <section id="my-artworks">
    <v-container v-intersect="onIntersect" fluid>
      <h2 :class="{'enter-up': isIntersecting }" class="poppins we-4 text-center text-uppercase">My artworks</h2>
      <v-divider :class="{'pop-out-divider': isIntersecting }" width="250rem" class="my-4 mb-7 mx-auto"></v-divider>
      <div :class="{'enter-up': isIntersecting }" class="d-none d-md-flex mx-auto justify-center flex-row flex-wrap">
        <div class="zoom-darken rounded-shaped ma-4 my-3" v-for="artwork in artworks">
          <img class="rounded-shaped" :src="artwork" width="200px" height="200px" />
        </div>
      </div>
      <v-carousel hide-delimiters class="mx-auto mt-16 d-md-none carousel-image" height="350px">
        <v-carousel-item class="zoom-darken" v-for="artwork in artworks">
          <img class="item-image" :src="artwork" />
          </v-carousel-item>
      </v-carousel>
    </v-container>
  </section>
</template>

<style scoped>
.item-image {
  object-fit: fill;
  width: 100%;
  height: 100%;
}
.carousel-image {
  background-size: 100% 100%;
  width: 320px;
}
.zoom-darken {
  overflow: hidden;
}
.zoom-darken img {
  transition: transform 1.3s ease, filter 0.8s ease;
  filter: grayscale(100%);
}
.zoom-darken:hover img {
  transform: scale(1.2);
  filter: grayscale(0%);
}
</style>
