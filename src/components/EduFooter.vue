<template>
  <footer class="flex">
      <div class="footer-themes flex flex-col">
          <div><span>Purchase</span></div>
          <div><span>Related</span></div>
      </div>

      <div class="footer-info flex flex-col">
          <EduLogo/>
          <p>EduPrime is the most versatile WordPress theme for
              educational purposes, showcasing universities, courses,
              secondary schools etc.
          </p>
          <div class="footer-icons">
              ICONS
          </div>
      </div>

      <div class="footer-nav flex">
          <nav>
              <h3>Get EduPrime</h3>
              <ul v-for="(item, index) in navLeft"
                    :key="index">
                <li>
                    <a href="#">
                        {{item.text}}
                    </a>
                </li>
              </ul>
          </nav>
          <nav>
              <h3>Networking</h3>
              <ul v-for="(item, index) in navRight"
                    :key="index">
                <li>
                    <a href="#">
                        {{item.text}}
                    </a>
                </li>
              </ul>
          </nav>
          
      </div>

      <div class="footer-search flex flex-col">
        <input class="search-bar" type="text" placeholder="Search...">
        <h4>Search Categories</h4>
        <div class="footer-tags flex">
            <ul class="flex">
                <li v-for="(item, index) in tags"
                :key="index" 
                class="category-tag">{{item}}</li>
            </ul>
        </div>
        <span>ModelTheme. All rights reserved.</span>

        <div class="arrow-up"></div>
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
    data () {
        return {
            navLeft: [
                {
                    id: 0,
                    text: "Request a website"
                },
                {
                    id: 1,
                    text: "Browse Themes"
                },
                {
                    id: 2,
                    text: "Payment Options"
                },
                {
                    id: 3,
                    text: "Support System"
                },
                {
                    id: 4,
                    text: "Checkout"
                },
                {
                    id: 5,
                    text: "Purchase Theme"
                },                
            ],
            navRight: [
                {
                    id: 0,
                    text: "Purchase Theme"
                },
                {
                    id: 1,
                    text: "Our Benefits"
                },
                {
                    id: 2,
                    text: "Our Team"
                },
                {
                    id: 3,
                    text: "Our Services"
                },
                {
                    id: 4,
                    text: "Other Products"
                },
                {
                    id: 5,
                    text: "My Account"
                },                
            ],
            tags: ["Economy", "Design", "Coaching", "Business", "Medicine", "Law", "Fitness"]
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
                border: 1px solid black;
                padding: 10px;
                margin: 10px;
                background-color: black;
                border-radius: 10px;
                width: 120px;
                font-size: 10px;
                text-align: center;
            }
        }

        .footer-info {
            justify-content: center;
            align-items: center;
            width: 25%;
        }

        .footer-nav {
            justify-content: space-around;
            align-items: center;
            width: 25%;

            a {
                color: white;
            }

        }

        .footer-search {
            justify-content: space-around;
            align-items: center;
            width: 40%;
            position: relative;

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
            }
        }

    }
    // Fine footer
</style>