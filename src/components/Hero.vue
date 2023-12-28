<script setup></script>

<template>
  <section>
    <v-container fluid class="ma-0 pa-0">
      <div class="image-container">
        <img class="banner-image w-100 h-screen" src="/background-1.jpg" />
        <div class="text-grey-lighten-1 w-100 text-placement">
          <v-row class="mt-n16 mt-sm-0 justify-center flex-column-reverse flex-sm-row" no-gutters>
            <v-col class="enter-down mx-2 text-center text-sm-right" sm="5" md="4" cols="12">
              <h2 class="poppins we-4 text-uppercase mt-4 mt-sm-0">A silly and improving artist</h2>
              <p>
                HII!&lt333 I’m a teen artist who’s improving as time passes! I love listening to
                music! Some of my favorite music artist are StrayKids, Eyedress, MacDemarco and
                Gorillaz! I enjoy watching anime or childhood cartoons like hunterXhunter, Tom and
                Jerry, a silent voice, etc. I love talking to my friends, both online and
                irl!!&lt333
              </p>
            </v-col>
            <v-divider class="d-flex d-sm-none"></v-divider>
            <v-divider class="d-none d-sm-flex ml-13 mr-4 divider-vertical" vertical></v-divider>
            <v-col class="enter-down align-self-center my-8 text-center" sm="5" cols="12">
              <p class="quote-text mx-16 mx-sm-0 font-italic">“Music speaks louder than words”</p>
              <p>Kousei Arima</p>
            </v-col>
          </v-row>
        </div>
      </div>
    </v-container>
  </section>
</template>

<style scoped>
.image-container {
  position: relative;
  background: rgb(0, 0, 0);
}
.banner-image {
  position: relative;
  opacity: 0.3;
  display: block;
  object-fit: cover;
}
.text-placement {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
h2 {
  font-size: 48px;
}
.quote-text {
  font-size: 37px;
}
</style>
