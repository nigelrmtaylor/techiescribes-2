<template>
  <div>
    <v-app-bar
      id="home-app-bar"
      class="pl-0"
      app
      prominent
      color="primary"
      elevation="1"
    >
      <v-col>
        <v-row dense>
          <v-col>
            <div
              class="display-2 font-weight-light mt-0 mb-auto align-stretch white--text"
            >
              TechieScribes
            </div>
          </v-col>
          <v-col>
            <v-app-bar-nav-icon
              class="hidden-md-and-up"
              @click="drawer = !drawer"
            />
          </v-col>
        </v-row>

        <v-row align-content="end">
          <v-col class="pt-0 pb-7">
            <div class="subtitle-1 font-weight-light white--text">
              Software Information Development & Localisation
            </div>
          </v-col>
        </v-row>
      </v-col>
      <template v-slot:extension class="extension-style">
        <v-tabs class="hidden-sm-and-down float-right" optional right>
          <v-tab
            v-for="item in items"
            :key="item.path"
            :to="item.path"
            nuxt
            :exact="true"
            :ripple="false"
            active-class="text--primary"
            min-width="96"
            text
          >
            {{ item.name }}
          </v-tab>
        </v-tabs>
      </template>
    </v-app-bar>

    <!-- <hr />
    <home-drawer v-model="drawer" :items="items" /> -->
  </div>
</template>

<script>
export default {
  name: 'AppBar',

  components: {
    // HomeDrawer: () => import('./Drawer')
  },

  data: () => ({
    drawer: null,
    items: [
      { name: 'Home', path: '/' },
      { name: 'Technical Documentation', path: '/services' },
      { name: 'Documentation Types', path: '/types' },
      { name: 'Localisation', path: '/locale' },
      { name: 'About', path: '/about' },
      { name: 'Contact', path: '/contact' }
    ]
  }) // data
}
</script>

<style>
.v-tab {
  text-transform: none !important;
}
</style>
