<template>
  <v-app>
    <div id="bg">
    <!-- Header -->
    <Header />
    <v-breadcrumbs
    large
    divider="/"
    :items="items"
    ></v-breadcrumbs>
    <v-divider/>
    <h1 class="h1">Datenflüsse beim Umzug</h1>

    <h3 class="h3">Was genau passiert mit Ihren persönlichen Daten bei der Anmeldung?</h3>

    <!-- Rows -->
    <div class="application">
    <v-container class="container">
      <!-- Row 1 -->
      <Row>
        <Placeholder>
          <DialogMStelle>
            <Knoten :src="require('@/assets/Node_MStelle.svg')" alt="mstelle" />
          </DialogMStelle>
        </Placeholder>
        <Placeholder />
        <Placeholder />
        <Placeholder />
        <Placeholder>
          <DialogGez>
            <Knoten :src="require('@/assets/Node_GEZ.svg')" alt="gez" />
          </DialogGez>
        </Placeholder>
      </Row>
      <!-- Row 2 -->
      <Row>
        <Placeholder />
        <Placeholder>
          <Pfeil :src="require('@/assets/oben_links.svg')" alt="arrow oben links" />
        </Placeholder>
        <Placeholder />
        <Placeholder>
          <Pfeil :src="require('@/assets/oben_rechts.svg')" alt="arrow oben rechts" />
        </Placeholder>
        <Placeholder />
      </Row>
      <!-- Row 3 -->
      <Row>
        <Placeholder />
        <Placeholder />
        <Placeholder>
          <DialogMReg>
            <Knoten :src="require('@/assets/Node_Mreg.svg')" alt="mreg" />
          </DialogMReg>
        </Placeholder>
        <Placeholder />
        <Placeholder />
      </Row>
      <!-- Row 4 -->
      <Row>
        <Placeholder />
        <Placeholder>
          <Pfeil :src="require('@/assets/unten_links.svg')" alt="arrow unten links" />
        </Placeholder>
        <Placeholder />
        <Placeholder>
          <Pfeil :src="require('@/assets/unten_rechts.svg')" alt="arrow unten rechts" />
        </Placeholder>
        <Placeholder />
      </Row>
      <!-- Row 5 -->
      <Row>
        <Placeholder>
          <DialogBeh>
            <Knoten :src="require('@/assets/Node_Behoerden.svg')" alt="behoerden" />
          </DialogBeh>
        </Placeholder>
        <Placeholder />
        <Placeholder />
        <Placeholder />
        <Placeholder>
          <DialogDritte>
            <Knoten :src="require('@/assets/Node_Dritte.svg')" alt="dritte" />
          </DialogDritte>
        </Placeholder>
      </Row>
    </v-container>
    <!-- Footer -->
    </div>
    <Footer/>
    </div>
  </v-app>
</template>

<script>
//nodes
import DialogMStelle from "@/components/DialogMStelle.vue";
import DialogGez from "@/components/DialogGez.vue";
import DialogMReg from "@/components/DialogMReg.vue";
import DialogBeh from "@/components/DialogBeh.vue";
import DialogDritte from "@/components/DialogDritte.vue";

//other
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import Placeholder from "@/components/Placeholder.vue";
import Pfeil from "@/components/Pfeil.vue";
import Knoten from "@/components/Knoten.vue";
import Row from "@/components/Row.vue";
import Dialog from "@/components/Dialog.vue";

export default {
  data:() => ({
    items: [
      {
        text: 'Bürgerservices',
        disabled: false
      },
      {
        text: 'Anmeldung',
        disabled: false
      },
      {
        text: 'Datenflüsse',
        disabled: true
      }
    ]
  }),
  name: "App",
  components: {
    Header,
    Footer,
    Placeholder,
    Knoten,
    Pfeil,
    Dialog,
    DialogMStelle,
    DialogGez,
    DialogMReg,
    DialogBeh,
    DialogDritte,
    Row,
  },
};
</script>

<style scoped>
.container {
  padding-left: 5px;
  padding-right: 5px;
  padding-bottom: 170px;
  background-color: whitesmoke;
}
.h1{
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  font-size: 1.9em;
  padding: 10px;
  padding-left: 20px;
}
.h3{
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  padding: 10px;
  padding-left: 20px;
  padding-bottom: 35px;
}
.application{
  align-self: left;
}
#app {
  background-color: whitesmoke;
  background-attachment: fixed;
}
</style>