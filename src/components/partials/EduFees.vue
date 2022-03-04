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
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi, suscipit porro. Ullam quis iure aut nulla obcaecati ipsam eos, nobis ducimus animi expedita, architecto tempora ipsum. Laudantium minima facere consectetur!</p>
                    <button class="main-btn brand-btn">List of Fees</button>
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
            border: 1px solid blue;
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