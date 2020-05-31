<template>
  <section id="welcome">
    <v-row no-gutters>
      <v-img
        :min-height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
        src="https://i.picsum.photos/id/1035/5854/3903.jpg"
      >
        <v-theme-provider>
          <v-container fill-height>
            <v-row align="center" class="white--text mx-auto" justify="center">
              <v-col class="black--text text-center" cols="12" tag="h1">
                <span
                  :class="[$vuetify.breakpoint.smAndDown ? 'display-2' : 'display-3']"
                  class="font-weight-light"
                >WELCOME TO</span>

                <br />

                <span
                  :class="[$vuetify.breakpoint.smAndDown ? 'display-3': 'display-4']"
                  class="font-weight-black"
                >MY SITE</span>
              </v-col>

              <v-btn class="align-self-end" fab outlined @click="$vuetify.goTo('#about-me')">
                <v-icon>mdi-chevron-triple-down</v-icon>
              </v-btn>
            </v-row>
          </v-container>
        </v-theme-provider>
      </v-img>
    </v-row>
  </section>
  <!-- <div class="home text-center">
    <img alt="Vue logo" src="../assets/logo.png" height="150" />
    <h1>Welcome to my page</h1>
  </div>-->
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {}
};
</script>
