<template>
  <v-app>
    <v-navigation-drawer app left color="#5e71c7" :width="325">
      <v-layout mt-10 column align-center>
        <v-avatar id="avatar" size="150">
          <img src="profile.jpg" alt="avatar" />
        </v-avatar>
        <v-list dense nav>
          <v-list-item>
            <v-list-item-content>About</v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-content>Education</v-list-item-content>
          </v-list-item>
        </v-list>
      </v-layout>
    </v-navigation-drawer>
    <v-toolbar dense color="#5e71c7" class="hidden-lg-and-up">
      <v-app-bar-nav-icon> </v-app-bar-nav-icon>
    </v-toolbar>

    <Resume />
  </v-app>
</template>

<script>
import Resume from '@/components/Resume'
import jump from 'jump.js'

export default {
  components: {
    Resume,
  },
  data() {
    return {
      items: [{ title: 'About' }, { title: 'Account' }, { title: 'Admin' }],
    }
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
