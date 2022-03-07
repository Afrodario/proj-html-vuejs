<template>
  <section class="newsletter">
      <div class="container flex">
          <h1>Subscribe Now to Our Newsletter!</h1>
          <div class="newsletter-input">
              <input class="search-bar" type="text" placeholder="Email address...">
              <button class="newsletter-button flex">
                  <font-awesome-icon icon="fa-solid fa-paper-plane" />
              </button>
          </div>
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

        .newsletter-input {
            position: relative;
            .newsletter-button {
                width: 55px;
                height: 55px;
                background-color: $buttonColor;
                border-radius: 50%;
                position: absolute;
                top: 0;
                right: 0;
                justify-content: center;
                align-items: center;
                color: white;
                font-size: 15px;
                border: none;
            }
        }
    }


}
</style>