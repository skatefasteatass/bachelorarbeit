<template>
    <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on, attrs }">
      <button class="dialog-trigger" v-bind="attrs" v-on.native="on">
        <slot />
      </button>
    </template>

    <v-card>
        <v-card-title>
          <h2 id="title" class="pa-2">Melderegister</h2>
          <v-spacer />
            <v-btn icon @click="dialog = false">
                <v-icon>mdi-close</v-icon>
            </v-btn>
        </v-card-title>

        <v-divider />

        <div class="content">
        Im <strong>Melderegister</strong> werden personenbezogene Daten von in einer Stadt angemeldeten Personen gespeichert. 
        Ein Melderegister wird von der zugehörigen Meldestelle einer Stadt verwaltet. <br>
        <br>
        Folgende personenbezogene Daten werden im Melderegister gespeichert:
        <ul>
            <li>Familienname</li>
            <li>frühere Namen</li>
            <li>Vornamen</li>
            <li>Doktorgrad</li>
            <li>Ordensname, Künsterlname</li>
            <li>personenbezogene Daten des gesetzlichen Vertreters</li>
            <li>Staatsangehörigkeiten</li>
            <li>rechtliche Zugehörigkeiten zu einer Religionsgesellschaft</li>
            <li>derzeitige und frühere Anschriften</li>
            <li>Einzugs- und Auszugsdaten</li>
            <li>Familienstand</li>
            <li>personenbezogene Daten zum Lebenspartner</li>
            <li>Ausstellungsbehörde, -datum, Gültigkeitsdauer und Seriennummer des Personalausweises</li>
            <li>AZR-Nummer unter dem Asylgesetz</li>
            <li>Auskunfts- oder Übermittlungssperren</li>
            <li>Sterbedatum und -ort</li>
        </ul>
        <br>
        Die <strong>EU-DSGVO</strong> (EU-Datenschutz-Grundverordnung) schreibt dabei vor, dass Daten aus dem Melderegister nur entsprechend der Aufgaben
        der Meldestellen verwendet werden dürfen. Die Meldestelle steht dabei in der Pflicht
        das Melderegister stets richtig und vollständig zu halten.<br>
        <br>
        Personen haben das Recht auf <strong>Auskunft</strong> über ihre Daten, 
        die Verarbeitungszwecke dieser Daten und ggfs. <strong>Berichtigung</strong> dieser Daten.
        Die Meldestellen müssen personenbezogene Daten <strong> löschen</strong>, 
        sofern diese zur Erfüllung ihrer Aufgabe nicht länger benötigt werden. <br>
        <br>
        Meldestellen dürfen anderen öffentlichen Stellen Daten aus dem Melderegister übermitteln, sofern dies
        zur Erfüllung der öffentlichen Aufgabe der entsprechenden Stelle dient. Diese Übermittlung 
        kann in regelmäßigen Abständen sowohl <strong>manuell</strong> als auch <strong>automatisiert</strong> erfolgen. <br>
        <br>
        Darüber hinaus können sog. <strong>Melderegisterauskünfte</strong> gestellt werden. 
        Dabei können Personen oder unabhängige dritte Institutionen die folgenden Daten zu einer Person anfragen:
        <ul>
            <li>Familienname</li>
            <li>frühere Namen</li>
            <li>Vorname</li>
            <li>Doktorgrad</li>
            <li>derzeitige Anschriften</li>
            <li>sofern die Person verstorben ist, diese Tatsache</li>
        </ul>
        <br>
        Werden diese Daten zu Gewerbezwecken verwendet, so müssen diese angegeben werden.
        Sie dürfen nicht außerhalb dieser Zwecke verwendet werden und müssen nach der Erfüllung ihres Zwecks gelöscht werden.
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
    name: "DialogMReg",
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