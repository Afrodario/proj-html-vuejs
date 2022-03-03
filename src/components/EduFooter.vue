<template>
  <footer class="debug flex">
      <div class="debug footer-themes flex flex-col">
          <div><span>Purchase</span></div>
          <div><span>Related</span></div>
      </div>

      <div class="debug footer-info flex flex-col">
          <EduLogo/>
          <p>EduPrime is the most versatile WordPress theme for
              educational purposes, showcasing universities, courses,
              secondary schools etc.
          </p>
          <div class="footer-icons">
              ICONS
          </div>
      </div>

      <div class="debug footer-nav flex">
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

      <div class="debug footer-search flex flex-col">
        <input class="search-bar" type="text" placeholder="Search...">
        <h4>Search Categories</h4>
        <div class="footer-tags flex">
            <ul v-for="(item, index) in tags"
                :key="index">
                <li class="category-tag">{{item}}</li>
            </ul>
        </div>
        <span>ModelTheme. All rights reserved.</span>
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
            align-items: center;
            width: 40%;
        }

    }
    // Fine footer
</style>