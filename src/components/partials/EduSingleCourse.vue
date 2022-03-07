<template>
  <div class="wrapper flex">
    <div v-for="(item, index) in latestCourses"
        :key="index"
        class="course flex">
        <img class="icon" :src="require('../../assets/img/' + item.path)">
        <h3>{{item.title}}</h3>
        <span>Teacher: {{item.teacher}}</span>
        <span>Price: {{item.price}}</span>
        <button class="main-btn brand-btn">View Course</button>
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
    border: 1px solid transparent;
    height: 200px;
    width: 200px;
    text-align: center;
    flex-direction: column;
    align-items: center;
    margin: 0 10px;
    justify-content: space-around;
    font-size: 14px;
}

</style>