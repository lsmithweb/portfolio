<template>
  <v-app light>
    <v-parallax :src="require('@/static/img/hero.jpeg')" height="600">
      <v-layout
        column
        align-center
        justify-center
      >
        <h1 class="hero text-center"></h1>
      </v-layout>
    </v-parallax>
    <section>
      <v-layout
        column
        wrap
        class="my-5"
        align-center
      >
        <v-flex xs12 class="my-3">
          <div>
            <h2 class="welcome my-2 display-1">Welcome To LSmith Web</h2>
            <hr>
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex>
                <v-card class="headline">
                  <v-card-text>
                    <p>Hey, I’m an freelance web developer from Phoenix, Arizona. I primarily work with JavaScript and frameworks such as <a href="https://expressjs.com/">Express</a> and <a href="https://nodejs.org/en/">Node.js</a>. See the <nuxt-link to="services" style="color: #00D1B2; text-decoration:none">Services page</nuxt-link> for more detail on what I do!</p>
                    <p class="sub">Need help with an upcoming project or application? Learn a bit more <nuxt-link to="about" style="color: #00D1B2; text-decoration:none">About Me</nuxt-link>  and then consider hiring me.</p>
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>
</v-app>
</template>

<script>
  import Logo from '@/components/Logo.vue'
  export default {
    components: {
      Logo
    }
  }
</script>
<style lang="stylus" scoped>
.hero
  height: 150px
  width: 100%
  background-image: url('~/static/img/clean-logo.svg')
.welcome
  font-weight: 300
  color: #35495e
  letter-spacing: 1px
  animation-delay: 1s
hr
  border: 0
  height: 1px
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0))
a
  color: #FC4445
  text-decoration: none
.headline
  max-width: 48rem
  font-weight: 300
  color: #526488
  word-spacing: 5px
  padding: 15px


</style>
