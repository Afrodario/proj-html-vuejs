<template>
  <div class="wrapper flex">
    <div v-for="(item, index) in latestCourses"
        :key="index"
        class="course flex">
        <img class="icon" :src="require('../../assets/img/' + item.path)">
        <h3>{{item.title}}</h3>
        <span>
        <font-awesome-icon icon="fa-regular fa-user" />
            Teacher: {{item.teacher}}
        </span>
        <span>
        <font-awesome-icon icon="fa-regular fa-money-bill-1" />
            Price: {{item.price}}
        </span>
        <button class="btn brand-btn">
        <font-awesome-icon icon="fa-regular fa-eye" />
            View Course
        </button>
    </div>
  </div>
</template>

<script>
export default {
    name: "EduSingleCourse",
    props: {
        latestCourses: Array,
    },
}

</script>

<style lang="scss" scoped>
.wrapper {
    justify-content: space-around;
}

.course {
    border: 1px solid lightgray;
    height: 200px;
    width: 200px;
    text-align: center;
    flex-direction: column;
    align-items: center;
    margin: 0 10px;
    justify-content: space-around;
    font-size: 14px;
    box-shadow: 1px 0px 3px 0px;
}

</style>