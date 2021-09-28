<template>
  <v-app dark>
    <v-app-bar app elevate-on-scroll color="white" height="90">
      <v-container class="align-center cols">
        <v-row >
          <v-col align="center">
            <v-btn depressed color="white">Home</v-btn>
            <v-btn depressed color="white">Blog</v-btn>
            <v-btn depressed color="white">Contact</v-btn>
          </v-col>
        </v-row>
      </v-container>
    </v-app-bar>
    <v-main>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>
