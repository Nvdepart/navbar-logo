<template>
  <div>
    <v-app-bar color="primary" dark>
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
        <v-row>
          <v-col
            cols="12"
            sm="6"
            md="4"
            v-for="video in popularVideos"
            :key="video.id"
          >
            <v-card>
              <v-img :src="video.thumbnail" aspect-ratio="16/9"></v-img>
              <v-card-title>{{ video.title }}</v-card-title>
            </v-card>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12">
            <v-card>
              <v-card-title class="headline">À propos de nous</v-card-title>
              <v-card-text>
                Nous sommes un couple passionné de nature et d'aventure qui
                parcourt le monde à la recherche des plus beaux endroits de
                notre planète. Nous partageons nos expériences sur notre chaîne
                YouTube afin de vous faire découvrir les merveilles de notre
                monde.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </div>
</template>

<script>
export default {
  data: () => ({
    popularVideos: [
      {
        id: 1,
        thumbnail: "https://youtu.be/Hmo0TmDvb9k",
        title: "Vidéo 1",
      },
      {
        id: 2,
        thumbnail: "https://example.com/thumbnail2.jpg",
        title: "Vidéo 2",
      },
    ],
  }),
};
</script>
