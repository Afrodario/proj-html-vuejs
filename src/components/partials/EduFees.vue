<template>
  <section class="fees">
      <div class="container">
          <div class="wrapper flex">
            <div class="fees-info fees-img">
                <img src="../../assets/img/Girl-Illustration.png">
            </div>
            <div class="fees-info fees-text">
                <img class="icon" src="../../assets/img/Exam-icon-1.png">
                <h1>Variables fees for international students</h1>
                <p class="text-regular">EduPrime has gathered teachers from around the globe to brainstorm in order to facilitate the evaluation of our students.
                    Every teacher from our university has an influence on how students are evaluated at his/her subject.</p>
                    <button class="btn brand-btn">List of Fees</button>
            </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "EduFees"
}
</script>

<style lang="scss" scoped>
section.fees {
    background-color: white;

    .wrapper {


        .fees-info {
            width: calc(100% / 2);
        }

        .fees-img {
            img {
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }
        
    }

}
</style>