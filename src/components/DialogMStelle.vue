<template>
  <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on, attrs }">
      <button class="dialog-trigger" v-bind="attrs" v-on.native="on">
        <slot />
      </button>
    </template>

    <v-card>
        <v-card-title>
          <h2 id="title" class="pa-2">Meldestelle</h2>
          <v-spacer />
            <v-btn icon @click="dialog = false">
                <v-icon>mdi-close</v-icon>
            </v-btn>
        </v-card-title>

        <v-divider />

            <div class="content">
              Die <strong>Meldestelle </strong> (Einwohnermeldeamt) registriert alle in einer Stadt lebenden Personen,
              um Identität und Wohnort eindeutig festhalten zu können. <br>
              <br>
              Meldestellen verwalten <strong>Melderegister</strong>, in welchen diese personenbezogenen Daten hinterlegt werden.<br>
              <br>
              Meldet man sich in einer neuen Stadt, an einer neuen Meldestelle an, 
              so ensteht ein <strong>Datenaustausch</strong> zwischen der Meldestelle des alten Wohnortes
              und der Meldestelle des neuen Wohnortes. 
              Dabei gleicht die neue Meldestelle
              ihre vorliegenden Daten mit den Daten der alten Meldestelle ab und überprüft diese auf Richtigkeit.<br>
              <br>
              Falls eine Persone <strong>mehrere</strong> Wohnungen besitzt, müssen alle Wohnungen angemeldet sein.<br>
              Eine dieser Wohnungen muss dabei als <strong>Hauptwohnung</strong> angemeldet sein. Alle für die 
              Wohnungen zuständigen Meldestellen erhalten dabei personenbezogenen Daten.
            </div>

        <v-divider/>

        <v-card-actions>
            <v-spacer />
                <v-btn color="primary" text @click="dialog = false">
                  {{ button }}
                </v-btn>
            <v-spacer />
        </v-card-actions>
    </v-card>
    </v-dialog>
</template>

<script>
export default {
    name: "DialogMStelle",
    props: {
    button: {
      type: String,
      default: "Schließen",
    },
  },
  data() {
    return {
      dialog: false,
    };
  },
}
</script>

<style scoped>
.dialog-trigger {
  width: 100%;
}
.content {
  text-align: block;
  font-size: 1.1em;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  margin-left: 8px;
  padding-left: 13px;
  padding-right: 18px;
  padding-bottom: 10px;
  padding-top: 10px;
}
#title {
  font-size: 1em;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
</style>