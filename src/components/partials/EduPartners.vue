<template>
  <section class="partners">
      <div class="container">
          <h1>Partners</h1>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio dignissimos reprehenderit ducimus fugiat deleniti cumque maxime, et repellat adipisci exercitationem provident, pariatur eum voluptas voluptates fuga qui eos quibusdam temporibus.</p>
        <div class="partners-logo flex">
            <div v-for="(item, index) in partners"
                :key="index" 
                class="part-logo">
                <img :src="require('../../assets/img/partner-' + item + '.png')">
            </div>
        </div>
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

    .container {
        text-align: center;

        .partners-logo {
            justify-content: space-around;

            .part-logo {
                

                img {
                    height: 100%;
                    object-fit: contain;
                    width: 100px;
                }
            }

        }
    }
}
</style>