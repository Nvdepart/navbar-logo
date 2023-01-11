<template>
  <footer class="footer">
    <div class="container">
      <div class="columns">
        <div class="column is-3">
          <h3 class="title is-5">Navigation</h3>
          <ul>
            <li><router-link to="/">Accueil</router-link></li>
            <li><router-link to="/videos">Vidéos</router-link></li>
            <li><router-link to="/playlists">Playlists</router-link></li>
            <li><router-link to="/about">A propos</router-link></li>
          </ul>
        </div>
        <div class="column is-3">
          <h3 class="title is-5">Abonnez-vous</h3>
          <p>
            Abonnez-vous à notre chaîne pour ne rien manquer des dernières
            vidéos !
          </p>
          <div class="field has-addons">
            <div class="control">
              <input type="text" class="input" placeholder="E-mail" />
            </div>
            <div class="control">
              <a class="button is-primary">S'abonner</a>
            </div>
          </div>
        </div>
        <div class="column is-3">
          <h3 class="title is-5">Suivez-nous</h3>
          <ul>
            <li><a href="https://www.facebook.com">Facebook</a></li>
            <li><a href="https://www.twitter.com">Twitter</a></li>
            <li><a href="https://www.instagram.com">Instagram</a></li>
            <li><a href="https://www.youtube.com">Youtube</a></li>
          </ul>
        </div>
        <div class="column is-3">
          <h3 class="title is-5">Contact</h3>
          <ul>
            <li>+34 6 32 34 36 58</li>
            <li>atlas-expo@gmail.com</li>
            <li>Av. Paisos Catalans 96, 17820 Girona</li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>
