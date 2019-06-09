<template lang="html">
  <div>
    <main>
      <AppFaq></AppFaq>
    </main>
  </div>

</template>

<script>
import AppFaq from '../components/AppFaq.vue';
export default {
  components: {
    AppFaq,
  },
}
</script>

<style lang="css" scoped>
main {
  margin: 2rem 3rem;
  font-family: Merriweather;
}
nav {
  font-family: Merriweather;
}
</style>
