<template>
  <section class="years">
      <div class="container">
          <div class="years-header">
              <img class="icon" src="../../assets/img/Clock-and-Bell.png">
              <h1>University Year</h1>
          </div>
          <div class="years-timeline">
              <div class="years-paragraph demo-p">
                  <h3>Demo Classes</h3>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
              </div>
              <div class="years-paragraph graduation-p">
                  <h3>Graduation Day</h3>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
              </div>
              <img id="timeline" src="../../assets/img/Timeline-Item.png">
              <div class="years-paragraph orientation-p">
                  <h3>Orientation</h3>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
              </div>
              <div class="years-paragraph evaluation-p">
                  <h3>Evaluation</h3>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
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

    .years-header {
        text-align: center;

        h1 {
            color: white;
            background-color: red;
            display: block;
            margin: 0 auto;
            width: 20%;
        }
    }

    .years-timeline {
        position: relative;

        .graduation-p {
            right: 5%;
        }

        .demo-p {
            left: 30%;
        }

        .evaluation-p {
            right: 25%;
            bottom: 5%;
        }

        .orientation-p {
            bottom: 5%;
            left: 10%;
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