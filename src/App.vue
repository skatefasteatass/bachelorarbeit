<template>
  <v-app>
    <Header />
    <!-- Row 1 -->
    <v-container class="container">
      <!-- Row 1 -->
      <Row>
        <Placeholder>
          <DialogMStelle>
            <Knoten :src="require('@/assets/Node_MStelle.svg')" alt="behoerden" />
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
          <Knoten :src="require('@/assets/oben_links.svg')" alt="arrow oben links" />
        </Placeholder>
        <Placeholder />
        <Placeholder>
          <Knoten :src="require('@/assets/oben_rechts.svg')" alt="arrow oben rechts" />
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
          <Knoten :src="require('@/assets/unten_links.svg')" alt="arrow unten links" />
        </Placeholder>
        <Placeholder />
        <Placeholder>
          <Knoten :src="require('@/assets/unten_rechts.svg')" alt="arrow unten rechts" />
        </Placeholder>
        <Placeholder />
      </Row>
      <!-- Row 5 -->
      <Row>
        <Placeholder>
          <DialogBeh>
            <Knoten :src="require('@/assets/Node_Behoerden.svg')" alt="mstelle" />
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
import Placeholder from "@/components/Placeholder.vue";
import Knoten from "@/components/Knoten.vue";
import Row from "@/components/Row.vue";
import Dialog from "@/components/Dialog.vue";

export default {
  name: "App",
  components: {
    Header,
    Placeholder,
    Knoten,
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
  padding-bottom: 5px;
  padding-top: 50px;
  padding-left: 5px;
  padding-right: 5px;
}
</style>