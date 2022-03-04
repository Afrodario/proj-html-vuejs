<template>
  <section class="newsletter">
      <div class="container flex">
          <h1>Subscribe Now to Our Newsletter!</h1>
          <input class="search-bar" type="text" placeholder="Email address...">
      </div>
  </section>
</template>

<script>
export default {
    name: "EduNewsletter"

}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
section.newsletter {
    background-color: $brandColor;
    height: 100px;

    .container {
        justify-content: space-around;
        align-items: center;
        height: 100px;
    }


}
</style>