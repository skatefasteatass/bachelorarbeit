<template>
  <v-app>
    <Header />
    <div style="">

      <!-- Row 1 -->
      <v-container>

    <!-- Row 1 -->
        <v-layout row justify-center>
          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/square.svg"
            alt="test"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/square.svg"
            alt="test"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"            
            >
            </v-img>
          </v-flex>
        </v-layout>

    <!-- Row 2 -->
        <v-layout row justify-center>
          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/oben_links.svg"
            alt="arrow upper left side"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/oben_rechts.svg"
            alt="arrow upper right side"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"            
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>
        </v-layout>

    <!-- Row 3 -->
        <v-layout row justify-center>
          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/square.svg"
            alt="test"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"            
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>
        </v-layout>

    <!-- Row 4 -->
        <v-layout row justify-center>
          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/unten_links.svg"
            alt="arrow lower left side"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/unten_rechts.svg"
            alt="arrow lower right side"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>
        </v-layout>

    <!-- Row 5 -->
        <v-layout row justify-center>

          <v-flex xs2>
            <v-img
            src="./assets/square.svg"
            alt="test"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"            
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2 >
            <v-img
            src="./assets/square.svg"
            alt="test"
            max-height="180px"
            max-width="180px"
            min-height="48px"
            min-width="48px"            
            >
            </v-img>
          </v-flex>
        </v-layout>

      </v-container>
    </div>
  </v-app>
</template>

<script>
import Header from './Components/Header.vue'

export default {
  name: 'App',
  components:{
    Header,
  },
};
</script>

<style scoped>
v-btn {
width:125px;
height:125px;
}
</style>>


