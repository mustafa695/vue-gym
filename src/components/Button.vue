<script setup>
defineProps({
  text: String,
  onClick: Function,
  btnClass: String,
});
</script>

<template>
  <button
    type="button"
    :class="`bg-black text-white px-7 py-2.5 rounded-[14px] ${btnClass}`"
    @click="onClick"
  >
    {{ text }}
  </button>
</template>
