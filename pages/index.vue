<template>
  <section>
    <header class="hero-image">
      <div class="hero-text">
        <h1>Merlin Movie House</h1>
      </div>
    </header>
    <main>
      <h2>A Cinematic Experience</h2>
      <p>Merlin Movie House is a place where all your film dreams come true. Ride a dragon, fight a jedi, kiss a toad...</p>
      <hr />
      <h2>Now Playing: Star Trek in its Entirety</h2>
      <div v-if="movies" class="flex-container">
        <!-- Checking data coming in
        <div style="display: block;">
          {{ movies }}
        </div> -->
        <!-- For loop through data from API search -->
        <div v-for="item in movies.Search">
          <div class="card" style="width: 18rem;">
            <img class="card-img-top" :alt="item.Title" :src="item.Poster">
            <div class="card-body">
              <h5 class="card-title">{{ item.Title }}</h5>
              <p>{{ item.Year }}</p>
              <!-- Booking link to nowhere until page is built -->
              <a href="#" class="btn btn-primary">Book Tickets</a>
            </div>
          </div>
        </div>
      </div>
    </main>
  </section>
</template>

<script>
import axios from 'axios';
export default {
  // API call
  data() {
    return {
      loading: true,
      movies: null,
      errored: false,
    };
  },
  mounted () {
    // Calling OMDBAPI
    axios.get('http://www.omdbapi.com/?s=star+trek&apikey=29917929')
      .then(response => (
        this.movies = response.data
      ))
      .catch(error => {
        console.log(error)
        this.errored = true
      })
      .finally(() => this.loading = false)
  }
}
</script>

<style scoped>
/* Styling for main hero image */
.hero-image {
  background-image: url('../assets/header.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
  position: relative;
  height: 600px;
  width: 100%;
}
/* Text laying over hero image */
.hero-text {
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
}
header h1 {
  font-family: Limelight, sans-serif;
  font-size: 5em;
  font-weight: bold;
  text-transform: uppercase;
  text-shadow: 2px 2px black;
}
main {
  margin: 2rem 3rem;
  font-family: Merriweather;
}
nav {
  font-family: Merriweather;
}

.flex-container {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  overflow: hidden;
  /* width: 100%; */
}

.flex-container div {
  padding: 0.5rem;
  margin: 0.5rem;
  width: 30%;
  font-size: 0.75rem;
  min-width: 200px;
}

</style>
