<template>
  <div class="my-bg-class">
    <v-container class="container">
      <NavBarChaine />

      <v-row>
        <v-col>
          <nuxt />
        </v-col>
      </v-row>
    </v-container>
    <Footer />
  </div>
</template>

<script>
import "bulma/css/bulma.css";
export default {
  name: "IndexPage",
};
</script>
<style>
.my-bg-class {
  background-image: url("~/static/bg-image.jpg");
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
