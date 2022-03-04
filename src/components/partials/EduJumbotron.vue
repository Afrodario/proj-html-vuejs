<template>
      <section class="jumbotron debug flex">
          <div class="container flex">
            <div class="jumbotron-text">
                <h1>Key to your Success</h1>
                    <p>EduPrime is the most versatile WordPress theme for
                        educational purposes, showcasing universities, courses,
                        secondary schools etc.
                    </p>
                <div class="jumbo-buttons">
                    <button class="main-btn">Search</button>
                    <button class="apply-btn">Apply for University</button>
                </div>
            </div>
          </div>
      </section>
</template>

<script>
export default {
    name: "EduJumbotron"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
.container {
        justify-content: center;
    }

    // Inizio jumbotron
    .jumbotron {
        background-color: $brandColor;
        height: 500px;
        justify-content: center;
        align-items: center;
        background: url("../../assets/img/theme_slider2_bg-1.jpg") center;

        .jumbotron-text {
            text-align: center;
            color: white;

                h1 {
                    font-size: 50px;
                    color: white;
                }

                p {
                    width: 60%;
                    margin: 20px auto;
                    font-size: 20px;
                }

            button {
                margin: 10px;
            }

        }
    }
    // Fine jumbotron
</style>