<script setup lang="ts">
import { ref, onMounted } from 'vue';
defineProps<{ options: object }>();
onMounted(() => {
  pq.grid(this.$el, this.options);
});
</script>

<template>
  <div :options="options"></div>
</template>

<style scoped></style>
