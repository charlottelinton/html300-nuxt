<template>
  <div>
    <AppNav/>
    <nuxt />
  </div>
</template>

<script>
// Importing nav for use across all pages
import AppNav from '../components/AppNav';

export default {
  components: {
    AppNav,
  }
}
</script>
