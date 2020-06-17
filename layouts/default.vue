<template>
  <div>
    <v-app>
      <app-bar />
      <!-- <v-app>
      <div>
        <hr />
        <hr />
      </div>
    </v-app> -->
      <v-content>
        <nuxt />
      </v-content>
      <footer-bar />
    </v-app>
  </div>
</template>

<script>
import AppBar from '@/components/AppBar'
import FooterBar from '@/components/FooterBar'

export default {
  name: 'Default',

  components: {
    AppBar,
    FooterBar
  },
  data: () => ({
    drawer: null,
    items: [
      { name: 'Home', path: '/' },
      { name: 'Technical Documentation', path: '/services' },
      { name: 'Documentation Types', path: '/types' },
      { name: 'Localisation', path: '/locale' },
      { name: 'Demo', path: '/demo' },
      { name: 'About', path: '/about' },
      { name: 'Contact', path: '/contact' }
    ]
  }) // data
}
</script>
