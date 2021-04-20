<template>
  <v-app>
    <v-navigation-drawer app permanent color="indigo lighten-3" :width="325">
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
