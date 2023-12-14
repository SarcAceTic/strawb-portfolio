<script setup>
const artworks = [
  'artwork_1.png',
  'artwork-2.png',
  'artwork-3.png',
  'artwork-4.png',
  'artwork-5.png',
  'artwork-6.png'
]
</script>

<template>
  <section>
    <v-container>
      <h2 class="poppins we-4 text-center text-uppercase">My artworks</h2>
      <v-divider width="250rem" class="my-4 mb-7 mx-auto"></v-divider>
      <div class="text-center d-flex flex-row flex-wrap">
        <div class="zoom-darken rounded-shaped ma-4 my-3" v-for="artwork in artworks">
          <img class="rounded-shaped" :src="artwork" width="200px" height="200px" />
        </div>
      </div>
    </v-container>
  </section>
</template>

<style scoped>
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
