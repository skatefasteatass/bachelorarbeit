<template>
  <v-app>
    <Header />
    <!-- Row 1 -->
    <v-container>
      <!-- Row 1 -->
      <Row>
        <Placeholder>
          <Dialog title="some title" text="some text">
            <Knoten :src="require('@/assets/Node_Behoerden.svg')" alt="test" />
          </Dialog>
        </Placeholder>
        <Placeholder />
        <Placeholder />
        <Placeholder />
        <Placeholder>
          <Dialog title="some title" text="some text">
            <Knoten :src="require('@/assets/Node_GEZ.svg')" alt="test" />
          </Dialog>
        </Placeholder>
      </Row>
      <!-- Row 2 -->
      <Row>
        <Placeholder />
        <Placeholder>
          <Knoten :src="require('@/assets/oben_links.svg')" alt="test" />
        </Placeholder>
        <Placeholder />
        <Placeholder>
          <Knoten :src="require('@/assets/oben_rechts.svg')" alt="test" />
        </Placeholder>
        <Placeholder />
      </Row>
      <!-- Row 3 -->
      <Row>
        <Placeholder />
        <Placeholder />
        <Placeholder>
          <Dialog title="some title" text="some text">
            <Knoten :src="require('@/assets/Node_Mreg.svg')" alt="test" />
          </Dialog>
        </Placeholder>
        <Placeholder />
        <Placeholder />
      </Row>
      <!-- Row 4 -->
      <Row>
        <Placeholder />
        <Placeholder>
          <Knoten :src="require('@/assets/unten_links.svg')" alt="test" />
        </Placeholder>
        <Placeholder />
        <Placeholder>
          <Knoten :src="require('@/assets/unten_rechts.svg')" alt="test" />
        </Placeholder>
        <Placeholder />
      </Row>
      <!-- Row 5 -->
      <Row>
        <Placeholder>
          <Dialog title="some title" text="some text">
            <Knoten :src="require('@/assets/Node_MStelle.svg')" alt="test" />
          </Dialog>
        </Placeholder>
        <Placeholder />
        <Placeholder />
        <Placeholder />
        <Placeholder>
          <Dialog title="some title" text="some text">
            <Knoten :src="require('@/assets/Node_Dritte.svg')" alt="test" />
          </Dialog>
        </Placeholder>
      </Row>
    </v-container>
  </v-app>
</template>

<script>
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
    Row,
  },
};
</script>

<style scoped>
v-btn {
  width: 125px;
  height: 125px;
}
</style>
>
