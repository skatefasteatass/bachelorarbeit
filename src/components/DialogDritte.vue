<template>
    <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on, attrs }">
      <button class="dialog-trigger" v-bind="attrs" v-on.native="on">
        <slot />
      </button>
    </template>

    <v-card>
         <v-card-title>
          <h2 id="title" class="pa-2">Dritte Institutionen</h2>
          <v-spacer />
            <v-btn icon @click="dialog = false">
                <v-icon>mdi-close</v-icon>
            </v-btn>
        </v-card-title>

        <v-divider />

        <div class="content">
        Sonstige (unabhängige) <strong>Dritte Institutionen</strong> sind nur indirekt von den Datenflüssen betroffen. Zu ihnen gehören beispielsweise 
        <strong>Parteien, Wählergruppen oder Adressbuchverlage</strong>. <br>
        <br>
        Über <strong>Melderegisterauskünfte</strong> haben unabhängige dritte Institutionen die Möglichkeit an personenbezogene Daten zu gelangen und diese zu verwenden. <br>
        <br>
        Personen haben dabei jedoch die Möglichkeit, über einen entsprechenden <strong>Antrag auf eine Auskunftssperre</strong> an eine Meldestelle der Weitergabe und Verarbeitung ihrer 
        personenbezogenen Daten zu widersprechen. Dieser Antrag muss ein Mal im jährlich gestellt werden. <br>
        </div>

        <v-divider />

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
    name: "DialogDritte",
    props: {
    button: {
      type: String,
      default: "Alles klar!",
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
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
</style>