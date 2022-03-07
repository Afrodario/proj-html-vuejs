<template>
  <section class="partners">
      <div class="container">
          <h1>Partners</h1>
          <p class="text-regular">Leverage agile frameworks to provide a robust synopsis for high level overviews. 
              Iterative approaches to corporate strategy.</p>
        <div class="partners-logo flex">
            <div v-for="(item, index) in partners"
                :key="index" 
                class="part-logo">
                <img :src="require('../../assets/img/partner-' + item + '.png')">
            </div>
        </div>
      </div>
      <div class="wave-container">
          <img src="../../assets/img/background-wave3.png">
      </div>
  </section>
</template>

<script>
export default {
    name: "EduPartners",
    data() {
        return {
            partners: [1, 2, 3, 4, 5, 6, 7, 8]
        }
    }
}
</script>

<style lang="scss" scoped>
section.partners {
    background-color: white;
    padding-top: 30px;

    .container {
        text-align: center;
        
        p {
            width: 40%;
            margin: 0 auto;
        }

        .partners-logo {
            justify-content: space-around;
            padding: 20px 0;

            .part-logo {
                margin: 10px;
                width: 200px;
                height: 50px;

                img {
                    height: 100%;
                    object-fit: contain;
                    width: 100%;
                    opacity: 0.4;
                }
            }

        }
    }
    .wave-container {
        height: 100px;
        img {
            width: 100%;
            height: 50%;
            }
    }
}
</style>