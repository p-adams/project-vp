<script setup>
import VideoPlayer from "./components/VideoPlayer.vue";
</script>

<template>
  <main>
    <header>
      <h3>Video Player Component Demo</h3>
    </header>
    <section></section>
    <footer></footer>
  </main>
  <VideoPlayer
    container-width="500px"
    container-height="500px"
    video-width="400px"
    video-height="400px"
  ></VideoPlayer>
</template>

<style scoped></style>
