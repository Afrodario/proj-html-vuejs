<template>
  <div id="app">
    <EduHeader/>
    <EduMain/>
    <EduFooter/>
  </div>
</template>

<script>
import EduHeader from './components/EduHeader.vue'
import EduMain from './components/EduMain.vue'
import EduFooter from './components/EduFooter.vue'

export default {
  name: 'App',
  components: {
    EduHeader,
    EduMain,
    EduFooter
  }
}
</script>

<style lang="scss">
// Importazione foglio di stile generale
@import "./assets/style/common.scss";
@import "./assets/style/variables.scss";


</style>
