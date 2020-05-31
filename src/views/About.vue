<template>
  <section id="about-me">
    <div class="text-center py-10">
      <v-avatar :size="[$vuetify.breakpoint.smAndDown ? '250' : '350']" class="grey darken-3">
        <img alt="Rane Gillian" src="../assets/logo.png" height="150" />
      </v-avatar>
      <h1
        class="font-weight-bold mt-5"
        :class="[$vuetify.breakpoint.smAndDown ? 'display-1' : 'display-2']"
      >ABOUT ME</h1>
      <v-divider style="width:180px" class="mx-auto mt-5 mb-1 grey darken-1"></v-divider>
      <v-divider style="width:180px" class="mx-auto mb-3 grey darken-1"></v-divider>

      <p
        class="mx-auto title container font-weight-light"
        style="max-width:750px"
      >Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos delectus perspiciatis, debitis, voluptatibus inventore reprehenderit accusantium ullam sed, iste amet error quaerat vel corrupti nemo velit deleniti saepe facilis magnam!</p>
      <v-btn class="align-self-end" fab outlined @click="$vuetify.goTo('#about-me')">
        <v-icon>mdi-chevron-triple-down</v-icon>
      </v-btn>
    </div>
  </section>
</template>

<script>
export default {
  name: "About"
};
</script>