<script setup>
defineProps({
  text: String,
  className: String,
});
</script>

<template>
  <h1 :class="`text-black font-bold md:text-[42px] text-3xl ${className}`">{{ text }}</h1>
</template>
