<template>
  <main class="debug">
      <EduJumbotron/>
      <EduCourses/>
      <EduFaculties/>
      <EduYears/>
      <EduEvents/>
      <EduLatestCourses/>
  </main>
</template>

<script>
import EduJumbotron from '../components/partials/EduJumbotron.vue'
import EduCourses from '../components/partials/EduCourses.vue'
import EduFaculties from '../components/partials/EduFaculties.vue'
import EduYears from '../components/partials/EduYears.vue'
import EduEvents from '../components/partials/EduEvents.vue'
import EduLatestCourses from '../components/partials/EduLatestCourses.vue'

export default {
    name: "EduMain",
    components: {
        EduJumbotron,
        EduCourses,
        EduFaculties,
        EduYears,
        EduEvents,
        EduLatestCourses
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
// Inizio main
main {
    background-color: blue;
}
// Fine main

</style>