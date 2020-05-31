<template>
  <v-app>
    <Header />
    <v-content>
      <!-- <router-view></router-view> -->
      <Home />
      <About />
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import Home from "@/views/Home";
import About from "@/views/About";

export default {
  name: "App",

  components: {
    Header,
    Footer,
    Home,
    About
  },

  data: () => ({
    //
  })
};
</script>
