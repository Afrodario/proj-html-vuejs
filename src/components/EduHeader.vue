<template>
  <header>
        <nav class="main-nav flex">
          <!-- Inizio parte sinistra navbar -->
            <EduLogo/>
          <!-- Fine parte sinistra navbar -->
          <!-- Inizio parte destra navbar -->
          <nav class="inner-nav flex">
              <ul v-for="(item, index) in innerNav"
                :key="index" 
              class="flex">
                  <li>
                      <a href="#">
                          {{item}}
                      </a>
                  </li>
              </ul>
              <button class="main-btn">View Courses</button>
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
    },
    data() {
        return {
            innerNav: [
                "Home",
                "Courses",
                "About Us",
                "News",
                "Pages",
                "Contact",
                "Purchase"
            ]
        }
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
            line-height: 50px;

            // Inizio inner nav
            .inner-nav {
                li {
                    a {
                        padding: 10px;
                        color: white;
                        font-weight: bold;
                    }
                }
            }
            // Fine inner nav
        }
        // Fine main nav
    }
    // Fine header
</style>