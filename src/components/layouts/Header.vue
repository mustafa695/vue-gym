<script setup>
import Button from "../Button.vue";
import Image from "../Image.vue";

const menu = ["Home", "About", "Trainers", "Review", "Plans"];
</script>

<template>
  <div class="wrapper flex gap-4 items-center py-4 z-50">
    <Image class="w-28 h-14 object-contain" url="src/assets/images/logo.png" />
    <div class="items-center gap-3 flex-1 justify-center md:flex hidden">
      <a
        href="#"
        v-for="(item, index) in menu"
        :key="index"
        :class="`text-black/40 font-normal p-2 ${index === 0 && '!text-black'}`"
        >{{ item }}</a
      >
    </div>

    <div class="flex justify-end w-full gap-4">
      <Button text="Join Now" />

      <button type="button" class="md:hidden">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 50 50"
          width="28px"
          height="28px"
        >
          <path
            d="M 0 7.5 L 0 12.5 L 50 12.5 L 50 7.5 Z M 0 22.5 L 0 27.5 L 50 27.5 L 50 22.5 Z M 0 37.5 L 0 42.5 L 50 42.5 L 50 37.5 Z"
          />
        </svg>
      </button>
    </div>
  </div>
</template>
