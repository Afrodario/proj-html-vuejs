<template>
  <section class="method">
      <div class="container">
          <div class="wrapper flex">
            <div class="method-info method-text">
                <img class="icon" src="../../assets/img/Exam-icon.png">
                <h1>The most efficient examination method</h1>
                <p class="text-regular">EduPrime has gathered teachers from around the globe to brainstorm in order to facilitate the evaluation of our students.
                    Every teacher from our university has an influence on how students are evaluated at his/her subject.
                </p>
                    <button class="btn brand-btn">Discover the method</button>
            </div>
            <div class="method-info method-img">
                <img src="../../assets/img/Exam-Illustration.png">
            </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "EduMethod"
}
</script>

<style lang="scss" scoped>
section.method {
    background-color: white;

    .wrapper {


        .method-info {
            width: calc(100% / 2);
        }

        .method-img {
            img {
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }
        
    }

}

</style>