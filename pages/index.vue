<template>
  <v-row>
    <v-col>
      <v-card>
        <v-navigation-drawer app>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="title">
                Richard's Resume
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-divider></v-divider>
        </v-navigation-drawer>
      </v-card>
    </v-col>
    <v-col>
      <div class="resume">
        <Resume />
      </div>
    </v-col>
  </v-row>
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
