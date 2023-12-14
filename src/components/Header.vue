<script setup>
import { ref } from 'vue'

let navDrawer = ref(false)
</script>

<template>
  <v-app-bar class="pa-2" elevation="4">
    <v-app-bar-title>
      <div class="d-flex align-center">
        <v-img max-height="35" max-width="35" src="/strawberryicon.png"></v-img>
        <h3 class="poppins ml-2 mr-1">Strawberry</h3>
        <h3 class="poppins text-purple">Chae</h3>
      </div>
    </v-app-bar-title>
    <v-btn class="d-none d-md-flex mx-2">Home</v-btn>
    <v-btn class="d-none d-md-flex mx-2">About</v-btn>
    <v-btn class="d-none d-md-flex mx-2">My Artworks</v-btn>
    <v-app-bar-nav-icon
      @click.stop="navDrawer = !navDrawer"
      class="d-flex d-md-none"></v-app-bar-nav-icon>
  </v-app-bar>
  <v-navigation-drawer location="right" v-model="navDrawer">
    <template v-slot:image>
      <v-img class="sass h-100" src="/someimage.jpg"></v-img>
    </template>
    <v-list class="mt-4">
      <v-list-item prepend-icon="mdi-home" link>
        <p class="text-button">
          home
        </p>
      </v-list-item>
      <v-list-item prepend-icon="mdi-account" link>
        <p class="text-button">
          about me
        </p>
      </v-list-item>
      <v-list-item prepend-icon="mdi-palette" link>
        <p class="text-button">
          my artworks
        </p>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<style scoped>
.sass {
 opacity: 0.4;
}
</style>