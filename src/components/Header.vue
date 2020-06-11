<template>
  <v-app-bar
    dark
    v-scroll="onScroll"
    :color="!isScrolling ? 'transparent' : ''"
    fixed
    flat
  >
    <!-- <v-img alt="Logo" contain max-height="30" max-width="30" :src="require('../assets/logo.png')" /> -->
    <v-toolbar-title>
      <span>RANE</span>
      <span class="font-weight-light">GILLIAN</span>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-btn
      icon
      href="https://www.facebook.com/ranegillian"
      target="_blank"
      class="mt-auto indigo darken-1 mx-1"
      v-bind="size"
    >
      <v-icon v-bind="size">mdi-facebook</v-icon>
    </v-btn>
    <v-btn
      icon
      href="https://github.com/rgvillanueva28"
      target="_blank"
      class="mt-auto black mx-1"
      v-bind="size"
    >
      <v-icon v-bind="size">mdi-github</v-icon>
    </v-btn>
    <v-btn
      icon
      href="https://www.linkedin.com/in/rane-villanueva-10a296154/"
      target="_blank"
      class="mt-auto indigo lighten-1 mx-1"
      v-bind="size"
    >
      <v-icon v-bind="size">mdi-linkedin</v-icon>
    </v-btn>
    <v-btn icon href="mailto:rgvillanueva28@gmail.com" class="mt-auto red mx-1" v-bind="size">
      <v-icon v-bind="size">mdi-gmail</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {
  name: "Header",
  computed: {
    size() {
      const size = { xs: "large", sm: "large", lg: "large", xl: "x-large" }[
        this.$vuetify.breakpoint.name
      ];
      return size ? { [size]: true } : {};
    }
  },
  data: () => ({
      isScrolling: false,
    }),
    methods: {
      onScroll () {
        const offset = window.pageYOffset
        this.isScrolling = offset > 50
      },
    },
};
</script>