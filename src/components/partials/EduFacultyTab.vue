<template>
<div class="wrapper flex">
  <div class="faculty-tab"
        v-for="(item, index) in facultiesList"
        :key="index">
        <img :src="require('../../assets/img/' + item.path)">
        <span>{{item.name}}</span>
  </div>
</div>
</template>

<script>
export default {
    name: "EduFacultyTab",
    props: {
        facultiesList: Array
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
.faculty-tab {
    height: 100%;
    width: calc(100% / 7);
    border: 1px solid black;
    display: inline-block;
    text-align: center;
    color: $brandColor;

    &:hover {
        background-color: $brandColor;
        color: white;
    }

    * {
        padding: 5px 0;
    }

    img {
    width: 70%;
    height: 70%;
    object-fit: contain;
    display: block;
    margin: 0 auto;
    }
}

.wrapper {
    justify-content: center;
}
</style>