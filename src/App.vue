<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <v-app>
    <Header />
    <v-main class="mt-4"><RouterView /></v-main>
    <Footer />
  </v-app>
</template>

<style scoped></style>
