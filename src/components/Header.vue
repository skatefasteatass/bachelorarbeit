<template>
<nav class="nav">
  <v-toolbar app elevation="2">
    <v-toolbar-title class="toolbar">
      <span class="font-weight-light">Stadt </span>
      <span>Musterstadt</span>
      <v-spacer />
            
    </v-toolbar-title>
    <v-icon>mdi-city-variant-outline</v-icon>
    <v-spacer />
    <v-btn flat color="grey">
      <span class="font-weight-light">Sign Out</span>
        <v-icon right color="grey lighten-2">
          mdi-account-circle
        </v-icon>
    </v-btn>
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
  margin-right: 2px;
}
</style>
