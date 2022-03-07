<template>
  <section class="latest-courses">
      <div class="container">
          <h1>Latest Courses</h1>
          <div class="courses-list flex">
              <EduSingleCourse :latestCourses="coursesList"/>
          </div>
      </div>
      

  </section>
</template>

<script>
import EduSingleCourse from './EduSingleCourse.vue'
export default {
    name: "EduLatestCourses",
    components: {
        EduSingleCourse,
    },
    data() {
        return {
            coursesList: [
                {
                    path: "Decisions-icon.png",
                    title: "Make Better Decisions",
                    teacher: "James Collins",
                    price: "$21.00"
                },
                {
                    path: "Speaker-icon.png",
                    title: "How to Be a Speaker",
                    teacher: "James Collins",
                    price: "Free"
                },
                {
                    path: "Network-icon.png",
                    title: "Network Introductions",
                    teacher: "James Collins",
                    price: "Free"
                },
                {
                    path: "Brand-icon.png",
                    title: "Brand Management",
                    teacher: "James Collins",
                    price: "Free"
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
section.latest-courses {
    background-color: white;
    padding-top: 100px;

    .courses-list {
        justify-content: space-around;
        align-items: center;
    }

}


</style>