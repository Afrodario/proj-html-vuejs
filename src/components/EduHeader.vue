<template>
  <header>
        <nav class="main-nav flex">
          <!-- Inizio parte sinistra navbar -->
            <EduLogo/>
          <!-- Fine parte sinistra navbar -->
          <!-- Inizio parte destra navbar -->
          <nav class="inner-nav flex">
              <ul v-for="(item, index) in innerNavHeader"
                :key="index" 
              class="flex">
                  <li>
                      <a href="#">
                          {{item.name}}
                      </a>
                      <font-awesome-icon v-if="item.dropdown==true"
                      icon="fa-solid fa-sort-down" />
                  </li>
              </ul>
              <button class="btn main-btn">VIEW COURSES</button>
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
    props: {
        innerNavHeader: Array
    },
    data() {
        return {
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
                    margin: 0 10px;
                    color: white;

                    a {
                        padding: 10px;
                        color: white;
                    }
                    
                }
            }
            // Fine inner nav
        }
        // Fine main nav
    }
    // Fine header
</style>