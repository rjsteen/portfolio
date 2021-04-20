<template>
  <v-container fill-height fluid>
    <v-row align="center" justify="center" class="d-flex align-center">
      <v-col cols="12" sm="6">
        <Presentation />
        <Education />
        <Experience />
        <Skills />
        <Interests />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Presentation from '../components/Sections/Presentation'
import Education from '../components/Sections/Education'
import Experience from '../components/Sections/Experience'
import Skills from '../components/Sections/Skills'
import Interests from '../components/Sections/Interests'

export default {
  components: {
    Presentation,
    Experience,
    Education,
    Skills,
    Interests,
  },
  methods: {},
}
</script>

<style></style>
