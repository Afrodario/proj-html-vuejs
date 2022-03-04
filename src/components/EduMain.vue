<template>
  <main class="debug">
      <EduJumbotron/>
      <EduCourses/>
      <EduFaculties/>
      <EduYears/>
      <EduEvents/>
      <EduLatestCourses/>
      <EduMethod/>
      <EduFees/>
      <EduNewsletter/>
  </main>
</template>

<script>
import EduJumbotron from '../components/partials/EduJumbotron.vue'
import EduCourses from '../components/partials/EduCourses.vue'
import EduFaculties from '../components/partials/EduFaculties.vue'
import EduYears from '../components/partials/EduYears.vue'
import EduEvents from '../components/partials/EduEvents.vue'
import EduLatestCourses from '../components/partials/EduLatestCourses.vue'
import EduMethod from '../components/partials/EduMethod.vue'
import EduFees from '../components/partials/EduFees.vue'
import EduNewsletter from '../components/partials/EduNewsletter.vue'


export default {
    name: "EduMain",
    components: {
        EduJumbotron,
        EduCourses,
        EduFaculties,
        EduYears,
        EduEvents,
        EduLatestCourses,
        EduMethod,
        EduFees,
        EduNewsletter
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