<template>
  <v-footer id="home-footer" color="primary" app>
    <v-container class="px-2 py-0 ma-0 fluid">
      <v-row>
        <v-col cols="6" md="6" class="pa-0">
          <div
            class="d-flex flex-wrap justify-md-start justify-center justify-md-none"
          >
            <template v-for="(s, i) in social">
              <div :key="s">
                <a
                  class="white--text caption pa-1 pa-md-0"
                  href="#"
                  v-text="s"
                />
              </div>
              <v-responsive
                v-if="i < social.length - 1"
                :key="`divider-${s}`"
                class="mx-4 shrink caption hidden-sm-and-down"
              >
                <v-divider vertical />
              </v-responsive>
            </template>
          </div>
        </v-col>

        <v-col
          class="white--text text-right text-md-right caption float-right white--text pa-1"
          cols="6"
          md="6"
        >
          Copyright &copy; 2020 TechieScribes.com Design by TechieScribes.com
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {
  name: 'HomeFooter',

  data: () => ({
    social: ['Facebook', 'Twitter', 'Linkedin']
  })
}
</script>

<style lang="sass">
#home-footer a
  text-decoration: none
</style>
