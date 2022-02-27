<template>
  <v-app>
    <Header />
    <div>
      <v-container>

    <!-- Row 1 -->
        <v-layout row justify-center>
          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-sheet color="blue" style="width:125px; height:125px">   </v-sheet>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-btn outline color="yellow" style="width:125px; height:125px" xs2 sm2 md2 lg2 xl2>
              <span>Knoten 2</span>
            </v-btn>
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
            max-height="125px"
            max-width="125px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/oben_rechts.svg"
            alt="arrow upper right side"
            max-height="125px"
            max-width="125px"
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
            <v-btn outline color="grey" style="width:125px; height:125px">
              <span>Knoten 3</span>
            </v-btn>
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
            max-height="125px"
            max-width="125px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/unten_rechts.svg"
            alt="arrow lower right side"
            max-height="125px"
            max-width="125px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>
        </v-layout>

    <!-- Row 5 -->
        <v-layout row justify-center>

          <v-flex xs2>
            <v-btn outline color="green" style="width:125px; height:125px">
              <span>Knoten 4</span>
            </v-btn>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2 >
            <v-btn outline color="red" style="width:125px; height:125px;">
              <span>Knoten 5</span>
            </v-btn>
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


