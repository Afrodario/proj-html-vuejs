<template>
  <section class="faculties">
      <div class="container">
          <div class="faculties-text">
            <h1>Faculties available at EduPrime</h1>
            <p class="text-regular">A single university with a load of courses, tailored
                to satisfy any student's needs.
            </p>
          </div>
      </div>

      <div class="slider">
        <div class="inner-slider flex">
            <EduFacultyTab :facultiesList="facultiesList"/>
        </div>
      </div>

        <div class="container faculty-active flex">
            <div class="faculty-selected-left">
                <img src="../../assets/img/Gavel-Illustration-e1556884768193.png" alt="Illustrazione Martelletto">
            </div>
            <div class="faculty-selected-right">
                <h1>Law Faculty</h1>
                <p class="text-regular">Learning from world leading academics and practicioners, you'll not only receive an outstanding
                    grounding in the theory of law, but you will be able to understand how those principles are applied in practice through
                    a range of student-led activities and competitions.
                </p>
                <button class="btn brand-btn">Read More</button>
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
    padding-bottom: 100px;

    .faculties-text {
        text-align: center;
    }

    .slider {
        border-top: 1px solid lightgray;
        border-bottom: 1px solid lightgray;

        .inner-slider {
            width: 80%;
            margin: 0 auto;
            justify-content: center;
        }
    }

    .faculty-selected-right {
        * {
            margin: 15px 0;
        }
    }

    .faculty-active {
        width: calc(100% / 2);
        padding-top: 30px;
    }
}
</style>