<template>
  <div id="app">
    <EduHeader :innerNavHeader="innerNavHeader"/>
    <EduMain/>
    <EduFooter :navLeftFooter="navLeftFooter"
                :navRightFooter="navRightFooter"
                :tagsFooter="tagsFooter"/>
  </div>
</template>

<script>
import EduHeader from './components/EduHeader.vue'
import EduMain from './components/EduMain.vue'
import EduFooter from './components/EduFooter.vue'
import "@fontsource/fredoka-one"

export default {
  name: 'App',
  components: {
    EduHeader,
    EduMain,
    EduFooter
  },
  data() {
    return {
            innerNavHeader: [
                {
                    dropdown: true,
                    name: "Home"
                },
                {
                    dropdown: true,
                    name: "Courses"
                },
                {
                    dropdown: false,
                    name: "About Us"
                },
                {
                    dropdown: true,
                    name: "News"
                },
                {
                    dropdown: true,
                    name: "Pages"
                },
                {
                    dropdown: false,
                    name: "Contact"
                },
                {
                    dropdown: false,
                    name: "Purchase"
                }
              ],
            navLeftFooter: [
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
            navRightFooter: [
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
            tagsFooter: ["Economy", "Design", "Coaching", "Business", "Medicine", "Law", "Fitness"]
    }
  }
}
</script>

<style lang="scss">
// Importazione foglio di stile generale
@import "./assets/style/common.scss";
@import "./assets/style/variables.scss";
body {
  font-family: "Fredoka One";
  font-weight: 100;
}

</style>
