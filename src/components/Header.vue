<template>
<nav class="nav">
  <v-toolbar app elevation="2">
    <v-toolbar-title class="toolbar">
      <span class="font-weight-light">Datenflüsse beim </span>
      <span>Umzug</span>


    </v-toolbar-title>
      <v-icon>mdi-home-switch</v-icon>
      <v-spacer />
      <span style="margin-right:5px">
        <v-avatar color="grey lighten-2" size="36">
          <v-icon dark>
            mdi-account-circle
          </v-icon>
        </v-avatar>
      </span>
  </v-toolbar>

</nav>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.nav {
  margin-bottom: 25px;
}
.toolbar {
  margin-left: 20px;
  margin-right: 2px;
}
</style>
