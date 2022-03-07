<template>
    <section class="courses">
        <div class="courses-banner">
            <a href="#">
                <span>Purchase EduPrime on Envato Market</span>
            </a>
        </div>
        <div class="container flex">
            <div class="courses-left">
                <div class="courses-text">
                    <img class="icon" src="../../assets/img/Books-icon.png" alt="Icona libri">
                    <h1>Thousands of courses for any type of student</h1>
                    <p class="text-regular">At EduPrime it doesn't matter what domain you wish to pursue a career in.
                        Here you can find a course that satisfies your needs within a click away and apply for a course
                        in a matter of minutes. EduPrime is ranked as the most versatile university in the world, thanks
                        to the number of courses it provides.
                    </p>
                    <button class="btn main-btn">Browse through courses</button>
                </div>
            </div>
            <div class="courses-right">
                <img src="../../assets/img/Graduation-Illustration.png" alt="Illustrazione Diploma">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "EduCourses"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
section.courses {
    background-color: white;

    .courses-banner {
        border: 1px solid black;
        background-color: black;
        max-width: 180px;
        max-height: 50px;
        font-size: 10px;
        text-align: center;
        padding: 5px;
        border-radius: 8px;
        margin-left: 10px;
        position: relative;

        a {
            color: white;
        }

        &::after {
            content: "";
            width: 0;
            height: 0;
            border-left: 10px solid transparent;
            border-right: 10px solid transparent;
            border-top: 10px solid black;
            position: absolute;
            bottom: -10px;
            left: 75px;
        }
    }

    .container {
        
        .courses-right {
            img {
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }

        .courses-text {
            width: 50%;
            padding: 20px;

            img, h1, p {
                padding: 10px 0;
            }
        }
    }

}
</style>