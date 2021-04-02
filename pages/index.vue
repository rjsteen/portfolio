<template>
  <section>
    <v-row justify="center" align="center">
      <v-col cols="12" sm="8" md="6">
        <div class="text-center">
          <logo />
          <vuetify-logo />
        </div>
        <v-card>
          <v-card-title class="headline">
            Welcome to the Vuetify + Nuxt.js template
          </v-card-title>
          <v-card-text>
            <p>
              Vuetify is a progressive Material Design component framework for
              Vue.js. It was designed to empower developers to create amazing
              applications.
            </p>
            <p>
              For more information on Vuetify, check out the
              <a
                href="https://vuetifyjs.com"
                target="_blank"
                rel="noopener noreferrer"
              >
                documentation </a
              >.
            </p>
            <p>
              If you have questions, please join the official
              <a
                href="https://chat.vuetifyjs.com/"
                target="_blank"
                rel="noopener noreferrer"
                title="chat"
              >
                discord </a
              >.
            </p>
            <p>
              Find a bug? Report it on the github
              <a
                href="https://github.com/vuetifyjs/vuetify/issues"
                target="_blank"
                rel="noopener noreferrer"
                title="contribute"
              >
                issue board </a
              >.
            </p>
            <p>Welcome folks!</p>
            <div class="text-xs-right">
              <em><small>&mdash; John Leider</small></em>
            </div>
            <hr class="my-3" />
            <a
              href="https://nuxtjs.org/"
              target="_blank"
              rel="noopener noreferrer"
            >
              Nuxt Documentation
            </a>
            <br />
            <a
              href="https://github.com/nuxt/nuxt.js"
              target="_blank"
              rel="noopener noreferrer"
            >
              Nuxt GitHub
            </a>
          </v-card-text>
          <v-card-actions>
            <v-spacer />
            <v-btn color="primary" nuxt to="/inspire"> Continue </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
    <div class="resume">
      <Resume />
    </div>
  </section>
</template>

<script>
import Resume from '@/components/Resume'
import jump from 'jump.js'

export default {
  components: {
    Resume,
  },
  head() {
    return {
      title: 'Richard Steen',
    }
  },
  methods: {
    jumpTo(element) {
      jump(element)
    },
  },
}
</script>

<style scoped>
h1 {
  font-size: 3rem;
  line-height: 5.5rem;
}
@media (min-width: 992px) {
  .resume {
    padding-top: 0;
    padding-left: 17rem;
  }
}
</style>
