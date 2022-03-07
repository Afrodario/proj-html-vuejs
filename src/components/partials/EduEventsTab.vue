<template>
  <div class="wrapper flex">
        <div v-for="(item, index) in sessionsDates"
            :key="index" 
            class="event">
            <h2>Coaching Sessions</h2>
            <span class="event-date text-regular">
            <font-awesome-icon icon="fa-solid fa-calendar-days" />
                {{item.date}}
            </span>
            <p class="text-regular">Lorem ipsum dolor sit amet, cosectetur adipiscit elit, sed do eiusmod tempor[...]</p>
            <button class="btn brand-btn">
            <font-awesome-icon icon="fa-solid fa-plus" />
                Find More
            </button>
        </div>
  </div>
</template>

<script>
export default {
    name: "EduEventsTab",
    props: {
        sessionsDates: Array
    }
}
</script>

<style lang="scss" scoped>
.wrapper {
    justify-content: space-around;

.event {
    height: 200px;
    width: 300px;
    background-color: white;
    border-radius: 20px;
    text-align: center;
    position: relative;

    h2, span, p {
        padding: 20px 0;
    }

    button {
        position: absolute;
        bottom: -25px;
        left: 30%;
    }
}
}

</style>