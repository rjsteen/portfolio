<template>
  <v-container fluid id="page-top">
    <v-card id="about">
      <Presentation />
    </v-card>
    <v-card id="education">
      <Education />
    </v-card>
    <v-card id="experience">
      <Experience />
    </v-card>

    <v-card id="skills">
      <Skills />
    </v-card>

    <v-card id="interests">
      <Interests />
    </v-card>
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
