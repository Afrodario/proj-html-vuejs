<template>
  <footer class="debug flex">
      <div class="debug footer-themes flex flex-col">
          <button>Purchase</button>
          <button>Related</button>
      </div>

      <div class="debug footer-info flex flex-col">
          <EduLogo/>
          <p>Lorem ipsum</p>
          <div class="footer-icons">
              ICONS
          </div>
      </div>

      <div class="debug footer-nav flex">
          <nav>
              <h3>Get EduPrime</h3>
              <ul>
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>Lorem</li>
              </ul>
          </nav>
          <nav>
              <h3>Networking</h3>
              <ul>
                  <li>Lorem</li>
                  <li>Lorem</li>
                  <li>Lorem</li>
              </ul>
          </nav>
          
      </div>

      <div class="debug footer-search flex flex-col">
        <input type="text" placeholder="Search...">
        <h4>Search Categories</h4>
        <div class="footer-tags flex">
            <ul>
                <li>Economy</li>
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
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
    // Inizio footer
    footer {
        height: 300px;
        background-color: $brandColor;

        div.debug {
            width: calc(100% / 4);
        }

        .footer-info {
            justify-content: center;
            align-items: center;
        }

        .footer-nav {
            justify-content: space-around;
            align-items: center;
        }

        .footer-search {
            align-items: center;
        }

    }
    // Fine footer
</style>