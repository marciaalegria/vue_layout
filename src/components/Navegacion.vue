<template>
  <v-row>
    <v-col
      v-for="(bar, i) in bars"
      :key="i"
      cols="12"
      sm="12"
      md="6"
      class="my-4"
    >
      <v-card
        color="grey lighten-4"
        flat
        height="200px"
      >
        <v-toolbar
          :color="bar.class"
          :dark="bar.dark"
        >
          <v-app-bar-nav-icon></v-app-bar-nav-icon>
          <v-toolbar-title>Mi App</v-toolbar-title>
          <v-spacer></v-spacer>
          <router-link to="/buscar">
            <v-btn icon>
            <v-icon>mdi-magnify</v-icon>
            </v-btn>
            </router-link>
            <router-link to="/grid">
              <v-btn icon>
              <v-icon>mdi-heart</v-icon>
              </v-btn>
            </router-link>

          <v-btn icon>
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </v-toolbar>
      </v-card>
    </v-col>
  </v-row>
</template>
<script>
  export default {
    data: () => ({
      bars: [
      
        { class: '', dark: true },
      ],
    }),
  }
</script>