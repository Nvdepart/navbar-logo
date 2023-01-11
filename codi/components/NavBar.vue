<template>
  <div class="navbar-brand">
    <v-app-bar class="navbar is-transparent" color="primary">
      <v-toolbar-title>Atlas Expo</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text>Accueil</v-btn>
      <v-btn text>Vidéos</v-btn>
      <v-btn text>Playlists</v-btn>
      <v-btn text>À propos</v-btn>
    </v-app-bar>
    <v-content>
      <v-container>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="6">
            <v-card>
              <v-card-title class="headline"
                >Bienvenue sur Atlas Expo</v-card-title
              >
              <v-card-text>
                Nous sommes une chaîne YouTube dédiée à la nature et à
                l'exploration de la planète. Rejoignez-nous pour des aventures
                inoubliables et des découvertes fascinantes.
              </v-card-text>
              <v-card-actions>
                <v-btn color="primary" text @click="subscribe">S'abonner</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </div>
</template>

<script>
export default {
  methods: {
    subscribe() {
      // Ajouter le code pour s'abonner à la chaîne ici
    },
  },
};
</script>
