<template lang="html">
  <div class="flex-container">
      <!-- Grabbing data from object in gallery.vue -->
      <div v-for="image in images" >
        <img v-bind:src="image.src" v-bind:alt="image.alt" class="img-thumbnail" data-toggle="tooltip">
        <div class="caption">
          <h3>{{ image.title }}</h3>
          <p>{{ image.description }}</p>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  props: ['images'],
  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
.flex-container {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  overflow: hidden;
  /* width: 100%; */
}

.flex-container div {
  padding: 0.5rem;
  width: 33%;
  font-size: 0.75rem;
  min-width: 200px;
}

.caption {
  width: 100%;
}

h3 {
  font-size: 1.2rem;
}
</style>
