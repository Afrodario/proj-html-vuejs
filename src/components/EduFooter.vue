<template>
  <footer class="flex">
      <div class="footer-themes flex flex-col">
            <div class="flex">
                <img src="../assets/svg/svg-3.svg">
              <span>Purchase Theme</span>
            </div>
            <div class="flex">
                <img src="../assets/svg/svg-2.svg">
              <span>Related Themes</span>
            </div>
      </div>

      <div class="footer-info flex flex-col">
          <EduLogo/>
          <p class="text-regular">EduPrime is the most versatile WordPress theme for
              educational purposes, showcasing universities, courses,
              secondary schools etc.
          </p>
          <div class="footer-icons">
              <ul>
                  <li>
                      <a href="#">
                        <font-awesome-icon icon="fa-brands fa-facebook-f" />
                      </a>
                  </li>
              </ul>
              <ul>
                  <li>
                      <a href="#">
                        <font-awesome-icon icon="fa-brands fa-twitter" />
                      </a>
                  </li>
              </ul>
              <ul>
                  <li>
                      <a href="#">
                        <font-awesome-icon icon="fa-brands fa-instagram" />
                      </a>
                  </li>
              </ul>
          </div>
      </div>

      <div class="footer-nav flex">
          <nav>
              <h3>Get EduPrime</h3>
              <ul v-for="(item, index) in navLeftFooter"
                    :key="index">
                <li class="text-regular">
                    <a href="#">
                        {{item.text}}
                    </a>
                </li>
              </ul>
          </nav>
          <nav>
              <h3>Networking</h3>
              <ul v-for="(item, index) in navRightFooter"
                    :key="index">
                <li class="text-regular">
                    <a href="#">
                        {{item.text}}
                    </a>
                </li>
              </ul>
          </nav>
          
      </div>

      <div class="footer-search flex flex-col">
        <div class="search-input">
            <input class="search-bar" type="text" placeholder="Search...">
            <button class="search-button flex">
                <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
            </button>
        </div>
        
        <h4>Search Categories</h4>
        <div class="footer-tags flex">
            <ul class="flex">
                <li v-for="(item, index) in tagsFooter"
                :key="index" 
                class="category-tag text-regular">{{item}}</li>
            </ul>
        </div>
        <span class="text-regular copyright">ModelTheme. All rights reserved.</span>

        <div class="arrow-up flex">
            <font-awesome-icon icon="fa-solid fa-chevron-up" />
        </div>
      </div>
  </footer>
</template>

<script>
import EduLogo from '../components/partials/EduLogo.vue'
export default {
    name: "EduFooter",
    components: {
        EduLogo,
    },
    props: {
        navLeftFooter: Array,
        navRightFooter: Array,
        tagsFooter: Array
    },
    data () {
        return {
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
    // Inizio footer
    footer {
        height: 300px;
        background-color: $brandColor;
        color: white;

        .footer-themes {
            justify-content: flex-end;

            div {
                align-items: center;
                justify-content: space-between;
                width: 125px;
                border: 1px solid black;
                padding: 10px;
                padding-right: 40px;
                margin: 10px;
                background-color: black;
                border-radius: 6px;
                width: 150px;
                font-size: 10px;
                text-align: center;

                img {
                    width: 10px
                }
            }
        }

        .footer-info {
            justify-content: space-evenly;
            width: 25%;

            .footer-icons {

                ul {
                    display: inline-block;
                    svg {
                    border: 2px solid $buttonColor;
                    padding: 10px;
                    border-radius: 50%;
                    margin: 10px;
                    width: 20px;
                    height: 20px;
                    color: white;
                    }
                }
            }
        }

        .footer-nav {
            justify-content: space-around;
            align-items: center;
            width: 25%;

            li {
                margin: 8px 0;
                
                a {
                    color: white;
                }

            }

        }

        .footer-search {
            justify-content: space-around;
            align-items: center;
            width: 40%;
            position: relative;

            .search-input {
                position: relative;
                .search-button {
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

            .arrow-up {
                width: 40px;
                height: 40px;
                background-color: $buttonColor;
                border-radius: 50%;
                position: absolute;
                right: 30px;
                bottom: 15px;
            }
        }

        .footer-tags {
            ul {
                flex-wrap: wrap;
                width: 70%;
                margin: 0 auto;
                justify-content: flex-end;
            }
        }

        .copyright {
            color: goldenrod;
        }

        .arrow-up {
            justify-content: center;
            align-items: center;
        }

    }
    // Fine footer
</style>