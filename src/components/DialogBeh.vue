<template>
    <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on, attrs }">
      <button class="dialog-trigger" v-bind="attrs" v-on.native="on">
        <slot />
      </button>
    </template>

    <v-card>
        <v-card-title>
          <h2 id="title" class="pa-2">Behörden und Ämter</h2>
          <v-spacer />
            <v-btn icon @click="dialog = false">
                <v-icon>mdi-close</v-icon>
            </v-btn>
        </v-card-title>

        <v-divider />

        <div class="content">
        Hat eine Person sich an einem neuen Wohnort angemeldet, werden die aktualisierten, 
        personenbezogenen Daten im Melderegister gespeichert. <br>
        <br>
        Nun können <strong>andere öffentliche Behörden und Ämter</strong> (wie beispielsweise <strong>Finanzamt, Gesundheitsamt, Passbehörde</strong>) Daten aus dem Melderegister übermittelt bekommen und diese verarbeiten.
        Umgekehrt haben diese Behörden und Ämter auch die Möglichkeit, Daten aus dem Melderegister anzufragen. <br>
        <br>
        Durch die <strong>EU-DSGVO </strong> (EU-Datenschutz-Grundverordnung) ist festgelegt, dass eine Datenübermittlung und -verarbeitung an anderen öffentlichen Behörden oder Ämtern
        nur erfolgen darf, wenn dies <strong>zur Erfüllung der öffentlichen Aufgaben</strong> dieser Behörden und Ämter dient. Ausnahmen sind dabei Strafverfolgung oder die Gefährdung der nationalen Sicherheit. <br>
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
    name: "DialogBeh",
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