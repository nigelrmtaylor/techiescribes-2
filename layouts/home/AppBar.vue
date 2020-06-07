<template>
  <div>
    <v-app-bar
      id="home-app-bar"
      app
      prominent
      src="https://picsum.photos/1920/1080?random"
      elevation="1"
    >
      <v-toolbar-title>Techiescribes</v-toolbar-title>
      <base-img
        :src="require('@/assets/logo.svg')"
        class="mr-3 hidden-xs-only"
        contain
        max-width="52"
        width="100%"
      />

      <base-img
        :src="require('@/assets/zero-logo-light.svg')"
        contain
        max-width="128"
        width="100%"
      />

      <v-spacer />

      <div>
        {{ items }}
        <v-tabs class="hidden-sm-and-down" optional>
          <v-tab
            v-for="(name, i) in items"
            :key="i"
            :to="{ name }"
            :exact="name === 'Home'"
            :ripple="false"
            active-class="text--primary"
            class="font-weight-bold"
            min-width="96"
            text
          >
            {{ name }}
          </v-tab>
        </v-tabs>
      </div>

      <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer" />
    </v-app-bar>

    <home-drawer v-model="drawer" :items="items" />
  </div>
</template>

<script>
export default {
  name: 'HomeAppBar',

  components: {
    HomeDrawer: () => import('./Drawer')
  },

  data: () => ({
    drawer: null,
    items: [
      'Home',
      'Technical Documentation',
      'Documentation Types',
      'Localisation',
      'About',
      'Contact'
    ]
  })
}
</script>

<style lang="sass"></style>
