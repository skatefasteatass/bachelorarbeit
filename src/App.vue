<template>
  <v-app>
    <div>
      <v-container style="margin-top:50px">

    <!-- Row 1 -->
        <v-layout row justify-center>
          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-sheet color="blue" style="width:100px; height:100px">   </v-sheet>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-btn outline color="yellow" style="width:100px; height:100px" xs2 sm2 md2 lg2 xl2>
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
            max-height="100px"
            max-width="100px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/oben_rechts.svg"
            alt="arrow upper right side"
            max-height="100px"
            max-width="100px"
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
            <v-btn outline color="grey" style="width:100px; height:100px">
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
            max-height="100px"
            max-width="100px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            <v-img
            src="./assets/unten_rechts.svg"
            alt="arrow lower right side"
            max-height="100px"
            max-width="100px"
            >
            </v-img>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>
        </v-layout>

    <!-- Row 5 -->
        <v-layout row justify-center>

          <v-flex xs2>
            <v-btn outline color="green" style="width:100px; height:100px">
              <span>Knoten 4</span>
            </v-btn>
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>

          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2>
            
          </v-flex>

          <v-flex xs2 sm2 md2 lg2 xl2 justify-left>
            <v-btn outline color="red" style="width:100px; height:100px">
              <span>Knoten 5</span>
            </v-btn>
          </v-flex>
        </v-layout>

      </v-container>
    </div>
  </v-app>
</template>

<script>

export default {
  name: 'App',
};
</script>
