<template>
  <div class="grid grid-cols-3 gap-4 mx-20 my-10">
   <MovieCard 
    v-for="movie in movies" 
    :key=movie
    :movie="movie"
   />
  </div>
</template>

<script setup>
import MovieCard from './MovieCard.vue';
const { movies } = defineProps({
    movies: Array
})
</script>
