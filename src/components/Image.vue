<script setup>
defineProps({
  url: String,
  class: String,
});
</script>

<template>
  <img :src="url" :class="class" alt="image"/>
</template>
