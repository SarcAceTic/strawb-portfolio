<script setup>
import { ref } from 'vue'

let isIntersecting = ref(false)

const onIntersect = (isInter, entries, observer) => {
  isIntersecting.value = isInter
}
</script>

<template>
  <section id="about-me">
    <v-container>
      <v-row v-intersect="onIntersect" class="flex-column-reverse flex-sm-row" no-gutters>
        <v-col  cols="10" sm="6" class="mx-auto" lg="6">
          <h2 :class="{ 'enter-right': isIntersecting }" class="poppins we-4 text-uppercase">About Me</h2>
          <v-divider :class="{ 'pop-out-divider': isIntersecting }" class="my-4" width="200rem"></v-divider>
          <p :class="{ 'enter-right': isIntersecting }" class="text-justify">
            I enjoy drawing many things but anime characters seem to be my favorite things to draw!
            I also love painting and coloring with ink or paint markers! I like creating things that
            could be useful in future or present! 
          </p>
          <p :class="{ 'enter-right': isIntersecting }" class="mt-4 text-justify">
            I enjoy most types of music but I mainly listen to
            indie rock or Kpop! I often listen to ‘Eyedress’ and ‘StrayKids’! My favorite song by
            eyedress is “Nice Girl from a Nice Part of Town” and for StrayKids, “3rd Eye” is my
            favorite! I’ve met a lot of amazing people online and irl so talking to them simply
            makes me happy!
          </p>
        </v-col>
        <v-divider :class="{ 'pop-out-divider': isIntersecting }" class="mx-4" vertical></v-divider>
        <v-col class="mx-sm-auto align-self-center mb-7" cols="7" sm="5" lg="5">
          <div class="d-flex align-center flex-column flex-lg-row">
            <v-avatar :class="{ 'pop-out': isIntersecting }" class="mr-4" size="250" image="/pfp.jpg"></v-avatar>
            <div :class="{ 'enter-left': isIntersecting }" class="d-flex flex-column">
              <div class="about-me-name mt-4 mt-lg mx-sm-auto mb-4 d-flex">
                <h3 class="poppins we-4 text-uppercase">strawberry</h3>
                <h3 class="poppins ml-1 we-4 text-uppercase text-purple-accent-1">chae</h3>
              </div>
              <div class="about-me-info mx-sm-auto d-flex flex-column">
                <p>
                  <b class="text-purple-accent-1">Pronouns</b>
                  : she/her
                </p>
                <p>
                  <b class="text-purple-accent-1">Age</b>
                  : Ask >:(
                </p>
                <p>
                  <b class="text-purple-accent-1">Nationality</b>
                  : American
                </p>
                <p>
                  <b class="text-purple-accent-1">Zodiac Sign</b>
                  : Sagittarius
                </p>
                <p class="mt-lg-6">
                  <b class="text-purple-accent-1">Hobbies</b>
                  : Art, crafting, music
                  <br />
                  & talking to friends!
                </p>
              </div>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.about-me-name {
  font-size: 25px;
}
</style>
