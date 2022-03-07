<template>
    <section class="courses">
        <div class="container flex">
            <div class="courses-left">
                <div class="courses-text">
                    <img class="icon" src="../../assets/img/Books-icon.png" alt="Icona libri">
                    <h1>Thousands of courses for any type of student</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae consectetur reiciendis ullam a! Itaque commodi aspernatur est rem autem assumenda, quasi possimus sed pariatur ullam nobis inventore quas provident omnis.</p>
                    <button class="main-btn">Browse through courses</button>
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