<script setup>
defineProps({
  heatLevel: Array,
});
const heatMap = {
  Hot: "🔥🔥🔥",
  Medium: "🔥🔥",
  Mild: "🔥",
};
</script>
<template>
  <span>
    {{ heatLevel ? heatMap[heatLevel] : "" }}
  </span>
</template>
