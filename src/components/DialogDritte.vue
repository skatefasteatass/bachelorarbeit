<template>
    <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on, attrs }">
      <button class="dialog-trigger" v-bind="attrs" v-on.native="on">
        <slot />
      </button>
    </template>

    <v-card>
         <v-card-title>
          <h2 id="title" class="pa-2">Außerbehördliche Institutionen</h2>
          <v-spacer />
            <v-btn icon @click="dialog = false">
                <v-icon>mdi-close</v-icon>
            </v-btn>
        </v-card-title>

        <v-divider />

        <div class="content">
        Sonstige (unabhängige) <strong>außerbehördliche Institutionen</strong> sind nur indirekt von den Datenflüssen betroffen. Zu ihnen gehören:
        <ul>
          <li>Parteien und Wählergruppen</li>
          <li>Adressbuchverlage</li>
          <li>öffentlich-rechtliche Religionsgesellschaften</li>
          <li>Mandatsträger, Presse und Rundfunk für Alters- und Ehejubiläen</li>
          <li>Bundesamt für Personalmanagement der Bundeswehr</li>
        </ul> 
        <br>
        Über <strong>Melderegisterauskünfte</strong> haben unabhängige dritte Institutionen die Möglichkeit an personenbezogene Daten zu gelangen und diese zu verwenden.
        Im Antrag auf eine Melderegisterauskunft muss dazu ein Zweck für die Melderegisterauskunft angegeben werden. Erhaltene Daten dürfen nur zu diesem angegebenen Zweck verwendet werden. <br>
        <br>
        Personen haben dabei jedoch die Möglichkeit, der <strong>Weitergabe</strong> ihrer personenbezogenen Daten 
        an unabhängige dritte Institutionen  zu <strong>widersprechen</strong>. Dies ist über einen formlosen, schriftlichen Antrag möglich. Eine Vorlage dazu wird auf vielen Bürgerservice-Webseiten bereitgestellt.<br>
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
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
font-size: 1em;
}
</style>