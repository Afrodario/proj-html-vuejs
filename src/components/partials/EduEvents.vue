<template>
  <section class="events">
      <div class="container">
          <div class="events-header">
              <img class="icon" src="../../assets/img/upcoming-events-calendar-icon.png">
              <h1>Upcoming Events</h1>
          </div>
          <div class="upcoming-events">
              <EduEventsTab :sessionsDates="sessionsDates"/>
              <div class="upcoming-btn flex">
                  <button class="main-btn">View All Events</button>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
import EduEventsTab from './EduEventsTab.vue'
export default {
    name: "EduEvents",
    components: {
        EduEventsTab
    },
    data() {
        return {
            sessionsDates: [
                {
                    id: 1,
                    date: "20 May 21:30 PM"
                },
                {
                    id: 2,
                    date: "24 Mar 18:00 PM"
                },
                {
                    id: 3,
                    date: "12 Feb 13:30 PM"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
section.events {
    background-color: $brandColor;
    height: 400px;

    .events-header {
        text-align: center;

        h1 {
            color: white;
            display: block;
            margin: 0 auto;
            width: 20%;
        }
    }

    .upcoming-events {
        justify-content: space-around;

        .upcoming-btn {
            justify-content: center;
            align-items: center;

            button {
                margin: 40px 0;
            }
        }

    }
}

</style>