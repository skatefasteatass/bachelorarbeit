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
              Die <strong>Meldestelle </strong> (auch Einwohnermeldeamt oder Bürgerservicebüro) registriert alle in einer Stadt lebenden Personen,
              um Identität und Wohnort eindeutig festhalten zu können.
              Meldestellen verwalten <strong>Melderegister</strong>, in welchen diese personenbezogenen Daten hinterlegt werden.<br>
              <br>
              Die Meldestelle ist der erste Anlaufpunkt nach einem Umzug.
              Für die Anmeldung des neuen Wohnortes benötigt die Meldestelle <strong>Personalausweis</strong> und die <strong>Wohngsgeberbestätigung</strong><br>
              <br>
              Anschließend erfolgt ein <strong>Datenaustausch</strong> zwischen der Meldestelle des <strong>alten Wohnortes</strong>
              und der Meldestelle des <strong>neuen Wohnortes</strong>. 
              Dabei gleicht die neue Meldestelle
              ihre vorliegenden Daten mit den Daten der alten Meldestelle ab und überprüft diese auf Richtigkeit.<br>
              <br>
              Falls eine Persone <strong>mehrere Wohnungen</strong> besitzt, müssen alle Wohnungen angemeldet sein.<br>
              Eine dieser Wohnungen muss dabei als <strong>Hauptwohnung</strong> angemeldet sein. Alle für diese 
              Wohnungen zuständigen Meldestellen erhalten dabei personenbezogene Daten des Mieters oder des Eigentümers. <br>
              
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