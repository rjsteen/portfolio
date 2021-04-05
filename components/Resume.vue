<template>
  <section id="page-top">
    <div class="container-fluid p-0">
      <section class="resume-section p-3 p-lg-5 d-flex d-column" id="about">
        <Presentation />
      </section>

      <section
        class="resume-section p-3 p-lg-5 d-flex flex-column"
        id="education"
      >
        <Education />
      </section>

      <section
        class="resume-section p-3 p-lg-5 d-flex flex-column"
        id="experience"
      >
        <Experience />
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="skills">
        <Skills />
      </section>

      <section
        class="resume-section p-3 p-lg-5 d-flex flex-column"
        id="interests"
      >
        <Interests />
      </section>
    </div>
  </section>
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
