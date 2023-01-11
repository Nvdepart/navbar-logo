<template>
  <v-navigation-drawer v-model="drawer" fixed>
    <v-toolbar flat>
      <v-toolbar-title transition="scale-transition"
        >Atlas-Expo</v-toolbar-title
      >
      <v-spacer></v-spacer>
      <v-btn icon @click.stop="drawer = !drawer">
        <v-icon>mdi-menu</v-icon>
      </v-btn>
    </v-toolbar>
    <v-list>
      <v-list-item v-for="item in items" :key="item.title" :to="item.link">
        <v-list-item-title>{{ item.title }}</v-list-item-title>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>
<script>
export default {
  data: () => ({
    drawer: true,
    items: [
      { title: "Accueil", link: "/" },
      { title: "Vidéos", link: "/videos" },
      { title: "Playlists", link: "/playlists" },
      { title: "À propos", link: "/about" },
    ],
  }),
};
</script>

<style>
.scale-transition {
  transition: all 0.3s ease-in-out;
}
.scale-transition:hover {
  transform: scale(1.1);
}
</style>
