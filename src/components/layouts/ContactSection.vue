<script setup>
import Image from "../Image.vue";
</script>

<template>
  <div class="pt-12 relative">
    <Image
      url="src/assets/images/contact.png"
      class="w-full sm:h-[400px] h-80 object-cover"
    />
    <div class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
      <p class="text-white sm:text-base text-xs text-center sm:pb-8 pb-2">Call us Today</p>
      <h2 class="text-white md:text-[56px] sm:text-[38px] text-2xl font-bold text-center">
        +1 - 5852826417
      </h2>
      <p class="text-center text-white/60 font-light md:text-lg sm:text-base text-sm sm:pt-6 pt-2">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis
      </p>
    </div>
  </div>
</template>
