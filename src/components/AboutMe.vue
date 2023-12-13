<script setup></script>

<template>
  <section>
    <v-container>
      <v-row no-gutters>
        <v-col lg="6">
          <h2 class="poppins we-4 text-uppercase">About Me</h2>
          <v-divider class="my-4" width="200rem"></v-divider>
          <p class="text-justify">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Corporis consequatur nemo
            cumque beatae cupiditate architecto, obcaecati exercitationem, commodi repellat harum
            quam quae impedit eos enim culpa, libero eligendi dolor. Laboriosam pariatur voluptatem
            quos dolore dicta. Cupiditate, recusandae ipsa magnam, labore architecto atque ipsum
            dolorem iusto at repellat totam fugit autem?
          </p>
          <p class="mt-4 text-justify">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam sunt numquam dolore amet
            harum ducimus! Sunt deserunt commodi beatae eveniet tempora consequuntur veritatis
            laborum rerum placeat, nulla quos amet quia!
          </p>
        </v-col>
        <v-divider class="mx-4" vertical></v-divider>
        <v-col class="align-self-center" lg="5">
          <div class="d-flex align-center flex-row">
            <v-avatar class="mr-4" size="250" image="/pfp.jpg"></v-avatar>
            <div class="d-flex flex-column">
              <div class="about-me-name mb-4 d-flex flex-row">
                <h3 class="poppins we-4 text-uppercase">strawberry</h3>
                <h3 class="poppins ml-1 we-4 text-uppercase text-purple">chae</h3>
              </div>
              <p><b class="text-purple">Pronouns</b>: she/her</p>
              <p><b class="text-purple">Age</b>: 14</p>
              <p><b class="text-purple">Nationality</b>: American</p>
              <p><b class="text-purple">Zodiac Sign</b>: Virgin</p>
            </div>
          </div>
          <p class="mt-6"><b class="text-purple">Hobbies</b>: Drawing, being dumb, and getting bullied by Sarc</p>
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
