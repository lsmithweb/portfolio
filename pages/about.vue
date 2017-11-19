<template>
  <v-app light>
        <v-container>
          <v-layout row wrap align-center>
            <v-flex xs12 md4>
              <div class="avt text-xs-center">
                <v-avatar size="250px">
                  <img
                    class="img-circle elevation-7"
                    src="~/static/img/engagement.jpg"
                  >
                </v-avatar>
                <h4 class="me display-1 my-2">Logan <strong>Smith</strong></h4>
                <p class=" me headline text-xs-center">You definitely want to hang out with me</p>
              </div>
            </v-flex>
            <v-flex xs12 md5 offset-md1>
              <div>
                <v-card hover>
                  <v-card-text class="subtitle">
                    <strong>Raised in the heat of Phoenix, Arizona with the snakes and scorpions.</strong> After years of working as a mechanic, I was ready to move on to something different. That's when I decided to join the United States Navy and travel the world. Over the 5 years that I served, I was fortunate to see different countries including Ireland, Germany, and Romania, as well as meeting my wonderful wife, Lauren, in Charleston, SC.
                    <br>
                    <br>
                    My favorite part of being a mechanic was always the <strong>diagnostics</strong> of a situation. Similarly, I became enthralled with the elegant dance between website <strong>design</strong> and <em>development</em>, and instantly fell in love with the strategic thinking of it all.
                    <br>
                    <br>
                    I primarily work with JavaScript and many of it's frameworks, however I am in the process of becoming proficient in PHP and Laravel. I am always learning and progressing to become a better developer.
                  </v-card-text>
                </v-card>
              </div>
            </v-flex>
          </v-layout>
        </v-container>
  </v-app>
</template>

<style lang="stylus" scoped>

.me
  color: #35495e

.subtitle
  color: #35495e

</style>
