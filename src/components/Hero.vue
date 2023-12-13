<script setup></script>

<template>
  <section>
    <v-container fluid class="ma-0 pa-0">
      <div class="image-container">
        <v-img class="banner-image w-100 h-auto" src="/background-1.jpg" />
        <div class="text-grey-lighten-1 w-100 text-placement">
          <v-row justify="center" no-gutters>
            <v-col class="text-right" xl="3" cols="4">
              <h2 class="poppins we-4 text-uppercase">A silly and improving artist</h2>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio quasi at dignissimos
                dolorum? Vel animi dicta, laudantium aliquid blanditiis consectetur hic ad odio!
                Quia at maxime iusto cum aperiam quisquam voluptate eos doloremque debitis? Quas,
                debitis culpa blanditiis facilis.
              </p>
            </v-col>
            <v-divider class="ml-13 mr-4" vertical></v-divider>
            <v-col class="align-self-center text-center" cols="4">
              <p class="quote-text font-italic">“Music speaks louder than words”</p>
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
