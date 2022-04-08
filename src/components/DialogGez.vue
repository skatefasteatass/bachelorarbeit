<template>
    <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on, attrs }">
      <button class="dialog-trigger" v-bind="attrs" v-on.native="on">
        <slot />
      </button>
    </template>

    <v-card>
        <v-card-title>
            <h2 id="title" class="pa-2">GEZ</h2>
            <v-spacer />
            <v-btn icon @click="dialog = false">
                <v-icon>mdi-close</v-icon>
            </v-btn>
        </v-card-title>

        <v-divider />

        <div class="content">
            Die <strong>GEZ</strong>, oder auch Beitragsservice von ARD, ZDF und Deutschlandradio, ist für den Einzug 
            der Rundfunkbeiträge zuständig. <br>
            <br>
            Durch den <strong>RBStV</strong> (Runfunkbeitragsstaatsvertrag) ist festgelegt, dass jede angemeldete, volljährige Person dazu verpflichtet ist, 
            vierteljährlich einen bestimmten Geldbetrag an die GEZ zu überweisen. In einem <strong>Haushalt mit mehreren Personen</strong>, wie beispielsweise 
            einer WG, muss nur eine Person den Rundfunkbeitrag zahlen.<br>
            Die dafür benötigten personenbezogenen Daten gelangen auf zwei verschiedene
            Arten zur GEZ: <br>
            <br>
            Bei der <strong>bundesweiten</strong> Meldedatenübermittlung (Meldedatenabgleich) senden alle Meldestellen die vorhandenen personenbezogenen Daten
            aller volljährigen Personen aus allen Melderegistern an die GEZ. 
            Die GEZ prüft diese Daten anschließend auf mögliche beitragspflichtige Personen. <br>
            <br>
            Bei einer <strong>anlassbezogenen</strong> Meldedatenübermittlung, wie beispielsweise einem <strong>Umzug</strong>,
            werden die neuen personenbezogenen Daten manuell an die GEZ übermittelt. <br>
            <br>
            Die GEZ erhält dabei Daten zu:
            <ul>
                <li>Familienname</li>
                <li>Vornamen</li>
                <li>früheren Namen</li>
                <li>Doktorgrad</li>
                <li>Familienstand</li>
                <li>Geburtsdatum</li>
                <li>aktuelle und letzte Anschrift von Haupt- und Nebenwohnung</li>
                <li>Einzugsdatum</li>
            </ul>
            <br>
            Durch die <strong>EU-DSGVO </strong> (EU-Datenschutz-Grundverordnung) ist festgelegt, dass diese Daten nur zur Erfüllung der Aufgabe verarbeitet werden dürfen, 
            zu der sie auch erhoben wurden. <br>
            <br>
            Durch die EU-DSGVO ist auch festgelegt, dass Personen das Recht auf <strong>Auskunft</strong>, <strong>Berichtigung</strong> 
            und ggfs. <strong>Löschung</strong> oder <strong>Einschränkung der Verarbeitung</strong> ihrer Daten haben. <br>
            Weitere Informationen zur EU-DSGVO gibt es <a href="https://dsgvo-gesetz.de/" target="_blank">hier</a>!<br>
            
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
    name: "DialogGez",
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