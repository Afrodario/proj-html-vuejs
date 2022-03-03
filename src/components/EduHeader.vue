<template>
  <header class="debug">
        <nav class="main-nav flex">
          <!-- Inizio parte sinistra navbar -->
            <EduLogo/>
          <!-- Fine parte sinistra navbar -->
          <!-- Inizio parte destra navbar -->
          <nav class="inner-nav">
              <ul class="flex">
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>
                      <button>View Courses</button>
                  </li>
              </ul>
          </nav>
          <!-- Fine parte destra navbar -->
        </nav>
  </header>
</template>

<script>
import EduLogo from '../components/partials/EduLogo.vue'

export default {
    name: "EduHeader",
    components: {
        EduLogo,
    }

}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
    // Inizio header
    header {
        height: 100px;
        background-color: $brandColor;

        // Inizio main nav
        .main-nav {
            justify-content: space-between;
            align-items: center;
            padding: 20px;
        }
        // Fine main nav
    }
    // Fine header
</style>