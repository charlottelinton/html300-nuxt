<template lang="html">
  <div>
    <!-- Bootstrap responsive navbar - collapses to hamburger menu -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <a class="navbar-brand" href="index.html">Merlin Movie House</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <nuxt-link class="nav-item nav-link" to="/">Home</nuxt-link>
          <nuxt-link class="nav-item nav-link" to="/Gallery">Gallery</nuxt-link>
          <nuxt-link class="nav-item nav-link" to="/About">About</nuxt-link>
          <nuxt-link class="nav-item nav-link" to="/faq">FAQ</nuxt-link>
        </div>
      </div>
    </nav>
  </div>

</template>

<script>
export default {
  name: 'AppNav'
}
</script>

<style lang="css" scoped>
</style>
