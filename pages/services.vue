<template>
  <v-app light>
    <section>
      <v-layout
        column
        wrap
        class="my-5"
        align-center
      >
        <v-flex xs12>
          <div>
            <h2 class="phrase animated fadeInLeft">My Expertise</h2>
          </div>
        </v-flex>
          <v-flex xs12>
            <v-container grid-list-md text-xs-center>
              <v-layout row wrap align-center>
                <v-flex xs12 md4 class="des animated fadeInLeft">
                  <v-card class="elevation-0 transparent">
                    <v-card-text>
                        <v-icon x-large class="gray--text text--lighten-2">create</v-icon>
                      </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="desc" offset-md1>Design</div>
                    </v-card-title>
                    <v-card-text>
                      <hr>
                      <p class="sub">I love to collaborate closely with my clients and tailor the design to their specific goals. Together we can find the exact style that you love, and what represents your business in the best way. Working with clients to understand them and their business is my favorite part of being a freelance web developer! My goal is to help businesses reach their potential and make an online impression.</p>
                    </v-card-text>
                  </v-card>
                </v-flex>
                  <v-flex xs12 md4 class="dev animated fadeInLeft">
                    <v-card class="elevation-0 transparent">
                      <v-card-text>
                          <v-icon x-large class="gray--text text--lighten-2">build</v-icon>
                        </v-card-text>
                      <v-card-title primary-title class="layout justify-center">
                        <div class="desc" >Development</div>
                      </v-card-title>
                      <v-card-text>
                        <hr>
                        <p class="sub">After we establish the layout and design principles that you want to achieve, I will get to work immediately. I am a full-stack developer, meaning that I am able to work on the entire project from design to production. Efficiency and punctuality is a key component of my development process. I understand that completing a task and getting your site up on time is essential! </p>
                      </v-card-text>
                    </v-card>
                  </v-flex>
                  <v-flex xs12 md4 class="sup animated fadeInLeft">
                    <v-card class="elevation-0 transparent">
                      <v-card-text>
                          <v-icon x-large class="gray--text text--lighten-2">favorite</v-icon>
                        </v-card-text>
                      <v-card-title primary-title class="layout justify-center">
                        <div class="desc" offset-md2>Support</div>
                      </v-card-title>
                      <v-card-text>
                        <hr>
                        <p class="sub">It is important that the owner of the website is able to understand how things work. This means that after your site is up and running, you won't be left to manage the site alone. If needed, I will show you how to conveniently update the content in your site, utilizing user friendly tools, such as Wordpress. If you ever need additional help, I am just a call away. Let's make something great!</p>
                      </v-card-text>
                    </v-card>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-flex>
          </v-layout>
        </section>

        <section>
          <v-parallax :src="require('@/static/img/lights.jpeg')" style="opacity: .8" height="380">
            <v-layout column align-center justify-center>
              <div class="headline white--text mb-3 text-xs-center">"We came to Logan in need of a website for our dog training business. Within just a few days he had the process moving and kept us in the loop every step of the way! I highly recommend him to anyone who needs a nice website for a reasonable price! 5 stars!"</div>
              <em>Austin Franklin</em>
            </v-layout>
          </v-parallax>
        </section>

        <section>
          <v-layout
            column
            wrap
            class="my-3"
            align-center
          >
            <v-flex xs12>
              <div class="text-xs-center">
                <h2 class="phrase">Some Tools I Use</h2>
              </div>
            </v-flex>
            <v-container class="tools" grid-list-md text-xs-center>
              <v-layout row wrap align-center>
                <v-flex xs12 md3 offset-md1>
                  <v-card class="elevation-0 transparent">
                    <v-card-title class="justify-center">
                      <div class="language">Front End</div>
                    </v-card-title>
                    <v-card-media>
                      <span><img src="~/static/img/html5.png"></span>
                      <span><img src="~/static/img/css3.png"></span>
                      <span><img src="~/static/img/sass.png"></span>
                      <span><img src="~/static/img/bootstrap.png"></span>
                    </v-card-media>
                  </v-card>
                </v-flex>
                <v-flex xs12 md3 offset-md1>
                  <v-card class="elevation-0 transparent">
                    <v-card-title class="justify-center">
                      <div class="language">Back End</div>
                    </v-card-title>
                    <v-card-media>
                      <span><img src="~/static/img/nodejs.png"></span>
                      <span><img src="~/static/img/express-js.png"></span>
                      <span><img src="~/static/img/mongodb-logo.png"></span>
                      <span><img src="~/static/img/phpLogo.svg"></span>
                      <span><img src="~/static/img/laravel.png"></span>
                    </v-card-media>
                  </v-card>
                </v-flex>
                <v-flex xs12 md3 offset-md1>
                  <v-card class="elevation-0 transparent">
                    <v-card-title class="justify-center">
                      <div class="language">JavaScript</div>
                    </v-card-title>
                    <v-card-media >
                      <span><img src="~/static/img/javascript.png"></span>
                      <span><img src="~/static/img/jquery.png"></span>
                      <span><img src="~/static/img/vue.jpg"></span>
                      <span><img src="~/static/img/angular.png"></span>
                    </v-card-media>
                  </v-card>
                </v-flex>
              </v-layout>
              </v-container>
              <v-flex xs12>
                <div>
                  <h2 class="display-2"><nuxt-link to="contact" style="text-decoration: none; color: #00D1B2">Let's Work Together!</nuxt-link></h2>
                </div>
              </v-flex>
              </v-layout>
            </v-container>
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
.phrase
  color: #35495e
  font-weight: 400
  font-size: 3.2rem
  margin: auto
  animation-delay: 0.75s
.sub
  color: #373737
  margin: auto
.desc
  color: #00D1B2
  font-weight: 400
  font-size: 1.8rem
  margin: auto
.language
  color: #FC4445
  font-weight: 400
  font-size: 1.8rem

hr
  border: 0;
  height: 0;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
  border-bottom: 1px solid rgba(255, 255, 255, 0.3)

.des
  animation-delay: 0.75s
.dev
  animation-delay: 0.50s
.sup
  animation-delay: 0.25s
.tools
  margin-right: 300px
</style>
