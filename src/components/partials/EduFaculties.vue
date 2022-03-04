<template>
  <section class="faculties">
      <div class="container">
          <div class="faculties-text">
            <h1>Faculties available at EduPrime</h1>
            <p>A single university with a load of courses, tailored
                to satisfy any student's needs.
            </p>
          </div>
      </div>

      <div class="slider">
        <div class="inner-slider flex">
            <EduFacultyTab :facultiesList="facultiesList"/>
        </div>
      </div>
  </section>
</template>

<script>
import EduFacultyTab from './EduFacultyTab.vue'
export default {
    name: "EduFaculties",
    components: {
        EduFacultyTab
    },
    data () {
        return {
            facultiesList: [
                {
                    path: "Gavel-v2.png",
                    name: "Law Faculty"
                },
                {
                    path: "Coins-tabs-v2.png",
                    name: "Economy"
                },
                {
                    path: "Medicine-tabs-v2.png",
                    name: "Medicine"
                },
                {
                    path: "Computer-tabs-v2.png",
                    name: "Computer Science"
                },
                {
                    path: "Palette-tabs-v2.png",
                    name: "Graphic Design"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
section.faculties {
    background-color: white;

    .faculties-text {
        text-align: center;
    }

    .slider {
        border: 1px solid gray;

        .inner-slider {
            width: 80%;
            margin: 0 auto;
            justify-content: center;
        }
    }
}
</style>