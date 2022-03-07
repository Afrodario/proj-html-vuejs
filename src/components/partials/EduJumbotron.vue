<template>
      <section class="jumbotron flex">
          <div class="container flex">
            <div class="jumbotron-text">
                <h1>Key to your Success</h1>
                    <p>EduPrime is the most versatile WordPress theme for
                        educational purposes, showcasing universities, courses,
                        secondary schools etc.
                    </p>
                <div class="jumbo-buttons">
                    <button class="main-btn">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                        Search courses
                    </button>
                    <button class="apply-btn">
                    <font-awesome-icon icon="fa-solid fa-user-plus" />
                        Apply for University
                    </button>
                </div>
            </div>
          </div>
            <div class="panel flex flex-col">
                <font-awesome-icon icon="fa-solid fa-cart-shopping" />
                <font-awesome-icon icon="fa-solid fa-book-open" />
                <font-awesome-icon icon="fa-solid fa-chart-pie" />
            </div>
            <div class="wave-container">
                <img src="../../assets/img/Wave-1.png">
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
        position: relative;

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

        .wave-container {
            position: absolute;
            bottom: -5px;

            img {
                width: 100%;
            }
        }

        .panel {
            left: 0;
            padding: 10px;
            position: absolute;
            background-color: $buttonColor;
            color: white;

            * {
                margin: 5px 0;
            }
        }

    }
    // Fine jumbotron
</style>