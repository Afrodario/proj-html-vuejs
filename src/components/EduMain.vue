<template>
  <main class="debug">
      <EduJumbotron/>
  </main>
</template>

<script>
import EduJumbotron from '../components/partials/EduJumbotron.vue'
export default {
    name: "EduMain",
    components: {
        EduJumbotron,
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
// Inizio main
main {
    height: 100vh;
    background-color: blue;
}
// Fine main

</style>