<template>
  <section class="method">
      <div class="container">
          <div class="wrapper flex">
            <div class="method-info method-text">
                <img class="icon" src="../../assets/img/Exam-icon.png">
                <h1>The most efficient examination method</h1>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi, suscipit porro. Ullam quis iure aut nulla obcaecati ipsam eos, nobis ducimus animi expedita, architecto tempora ipsum. Laudantium minima facere consectetur!</p>
                    <button class="main-btn brand-btn">Discover the method</button>
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
            border: 1px solid blue;
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