<template>
  <section class="years">
        <div class="wave-container">
            <svg version="1.0" xmlns="http://www.w3.org/2000/svg" width="2954.667" height="186.667" viewBox="0 0 2216 140"><path class="st0" d="M324.7 34.8c-76.4 51.8-134.1 82-177.2 92.8-12.2 3.1-33.8 4.3-42.8 2.5-8.1-1.7-18.5-7.2-24.2-12.8-5.7-5.7-10.1-12.2-17.4-26.1C57 79.6 52.6 75 47.7 75c-7.9 0-21.2 9.9-37.9 28.3L0 114v26h1105.2c729.3 0 1104.9-.3 1104.2-1-2.6-2.6-29.5-18-42.9-24.5-46.4-22.7-82.1-27.7-122.7-17.5-4.6 1.2-19.1 5.5-32.3 9.5-40.2 12.4-58.5 16.1-85.5 17.2-33.9 1.3-73.5-5.3-117.9-19.9-14.8-4.8-48.5-17.8-59.7-23l-5.2-2.4-16.3 1.8c-125.9 13.6-219.6 20.5-324.9 23.9-40.1 1.3-166.2.6-196-1-71.9-4-119.7-8.4-173.5-16.2-26.8-3.8-69.6-11.2-83.1-14.4-5-1.1-8-1.3-13.2-.5-3.7.5-18.8 2.3-33.7 3.9C793 88.1 702 89.1 622 79c-51.2-6.5-89.6-15.2-150.5-34-35.4-10.9-84.3-20.7-121.8-24.3-3.5-.3-5.6.9-25 14.1z" fill="#e56768"/></svg>
        </div>
        <div class="container">
            <div class="years-header">
                <img class="icon" src="../../assets/img/Clock-and-Bell.png">
                <h1>University Year</h1>
            </div>
            <div class="years-timeline">
                <div class="years-paragraph demo-p">
                    <h3>Demo Classes</h3>
                    <p class="text-regular">In the first week, students try to accomodate with the teaching style and choose their optional courses.</p>
                </div>
                <div class="years-paragraph graduation-p">
                    <h3>Graduation Day</h3>
                    <p class="text-regular">On the day of graduation, all students gather for the ceremony and then network and party among others.</p>
                </div>
                <img id="timeline" src="../../assets/img/Timeline-Item.png">
                <div class="years-paragraph orientation-p">
                    <h3>Orientation</h3>
                    <p class="text-regular">First day of the university year, all students gather for the opening ceremony and then network with others.</p>
                </div>
                <div class="years-paragraph evaluation-p">
                    <h3>Evaluation</h3>
                    <p class="text-regular">At the end of a semester, students take a general evaluation test for every subject they're learning.</p>
                </div>
            </div>
        </div>
  </section>
</template>

<script>
export default {
    name: "EduYears"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
section.years {
    background-color: $brandColor;
    height: 500px;

    .wave-container {
        position: relative;

        svg {
            width: 100%;
            position: absolute;
            top: -142px;
        }
    }

    .years-header {
        text-align: center;

        h1 {
            color: white;
            background-color: red;
            display: block;
            margin: 30px auto;
            width: 20%;
        }
    }

    .years-timeline {
        position: relative;

        .graduation-p {
            right: 13%;
        }

        .demo-p {
            left: 30%;
        }

        .evaluation-p {
            right: 31%;
            bottom: 0;
        }

        .orientation-p {
            bottom: 0;
            left: 13%;
        }
    }

    #timeline {
        margin: 0 70px;
        display: block;
        padding: 70px 0;
    }

    .years-paragraph {
        display: inline-block;
        width: 20%;
        position: absolute;
        color: white;
        text-align: center;
        font-size: 13px;
    }
}

</style>