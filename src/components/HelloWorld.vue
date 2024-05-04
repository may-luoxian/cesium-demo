<template>
  <div id="cesiumContainer"></div>
</template>

<script setup lang="ts">
import { onMounted } from "vue";
import * as Cesium from "cesium";

onMounted(() => {
  let viewer = new Cesium.Viewer("cesiumContainer");
  console.log(viewer)
});
</script>

<style scoped>
#cesiumContainer {
  width: 100%;
  height: 100%;
  overflow: hidden;
}
</style>
