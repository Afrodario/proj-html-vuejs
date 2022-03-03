<template>
  <main class="debug">
      <section class="jumbotron debug flex">
          <div class="jumbotron-text">
              <h1>Key to your Success</h1>
              <p>Lorem ipsum</p>
              <div class="jumbo-buttons">
                  <button>Search</button>
                  <button>Apply</button>
              </div>
          </div>
      </section>
  </main>
</template>

<script>
export default {
    name: "EduMain"
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
// Inizio main
main {
    height: 100vh;
    background-color: blue;

    // Inizio jumbotron
    .jumbotron {
        background-color: $brandColor;
        height: 400px;
        justify-content: center;
        align-items: center;
    }
    // Fine jumbotron
}
// Fine main

</style>