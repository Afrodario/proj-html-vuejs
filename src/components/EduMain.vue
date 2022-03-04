<template>
  <main class="debug">
      <EduJumbotron/>
      <EduCourses/>
      <EduFaculties/>
      <EduYears/>
  </main>
</template>

<script>
import EduJumbotron from '../components/partials/EduJumbotron.vue'
import EduCourses from '../components/partials/EduCourses.vue'
import EduFaculties from '../components/partials/EduFaculties.vue'
import EduYears from '../components/partials/EduYears.vue'
export default {
    name: "EduMain",
    components: {
        EduJumbotron,
        EduCourses,
        EduFaculties,
        EduYears
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