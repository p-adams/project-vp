<script setup>
const props = defineProps({
  containerWidth: String,
  containerHeight: String,
  videoWidth: String,
  videoHeight: String,
});
function setWidthHeight(width, height) {
  return { width, height };
}
</script>

<template>
  <div
    class="Video-player-container"
    :style="setWidthHeight(containerWidth, containerHeight)"
  >
    <video
      class="Video-element"
      :style="setWidthHeight(videoWidth, videoHeight)"
    ></video>
    <slot></slot>
  </div>
</template>

<style scoped>
.Video-player-container {
  border: 1px solid gray;
}
.Video-element {
  border: 1px solid gray;
}
</style>
