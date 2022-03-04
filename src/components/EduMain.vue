<template>
  <main class="debug">
      <EduJumbotron/>
      <EduCourses/>
  </main>
</template>

<script>
import EduJumbotron from '../components/partials/EduJumbotron.vue'
import EduCourses from '../components/partials/EduCourses.vue'
export default {
    name: "EduMain",
    components: {
        EduJumbotron,
        EduCourses
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