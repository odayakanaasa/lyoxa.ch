<template>
  <nav class="navbar sticky-top navbar-expand-md navbar-light bg-white mb-5 border border-top-0 border-right-0 border-left-0">
    <div class="container">
      <nuxt-link to="/" class="navbar-brand" @click.native="closeMenu()">
        <img src="/img/logo.svg" width="73" height="30" alt="Lyoxa's logo">
      </nuxt-link>

      <button class="navbar-toggler hamburger hamburger--minus" type="button" data-toggle="collapse" data-target="#navbarToggler" aria-controls="navbarToggler" aria-expanded="false" aria-label="Toggle navigation">
        <span class="hamburger-box">
          <span class="hamburger-inner"></span>
        </span>
      </button>

      <div class="collapse navbar-collapse" id="navbarToggler">
        <ul class="navbar-nav ml-auto mt-2 mt-md-0">
          <li class="nav-item">
            <nuxt-link to="/" class="nav-link" exact @click.native="closeMenu()">Accueil</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link to="/lyoxa/" class="nav-link" @click.native="closeMenu()">Lyoxa</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link to="/services/" class="nav-link" @click.native="closeMenu()">Services</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link to="/equipe/" class="nav-link" @click.native="closeMenu()">Équipe</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link to="/partenaires/" class="nav-link" @click.native="closeMenu()">Partenaires</nuxt-link>
          </li>
          <!-- <li class="nav-item">
            <nuxt-link to="/portfolio" class="nav-link" @click.native="closeMenu()">Portfolio</nuxt-link>
          </li> -->
          <li class="nav-item">
            <nuxt-link to="/contact/" class="nav-link" @click.native="closeMenu()">Contact</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link to="/formulaire-de-demande/" class="nav-link--cta btn btn-primary" @click.native="closeMenu()">Nouvelle demande</nuxt-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  methods: {
    closeMenu: function () {
      /* eslint no-undef: off */
      $('#navbarToggler').collapse('hide')
    }
  }
}
</script>
