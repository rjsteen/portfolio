<template>
  <v-app>
    <v-row app>
      <v-col md="2">
        <v-navigation-drawer permanent color="blue darken-2" class="rounded-0">
          <v-list class="justify-center">
            <div class="d-flex justify-center">
              <v-avatar id="avatar" size="130">
                <img src="profile.jpg" alt="avatar" />
              </v-avatar>
            </div>

            <v-list-item v-for="item in items" :key="item.title" link>
              <v-list-item-content>
                <v-list-item-title class="d-flex justify-center">{{
                  item.title
                }}</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-navigation-drawer>
      </v-col>
      <v-col>
        <Resume />
      </v-col>
    </v-row>
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
