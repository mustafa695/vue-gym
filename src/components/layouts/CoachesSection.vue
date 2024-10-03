<script setup>
import Button from "../Button.vue";
import Image from "../Image.vue";
import MainHeading from "../MainHeading.vue";
</script>

<template>
  <div class="flex lg:flex-row flex-col lg:items-stretch lg:gap-4 gap-10 wrapper mt-28 mb-20">
    <div class="lg:w-2/5 w-full lg:min-w-max">
      <div class="flex items-stretch gap-4">
        <Image
          url="/assets/images/coach-1.jpeg"
          class="lg:w-[160px] w-2/5 h-[260px] object-cover rounded-xl shadow-sm drop-shadow-md "
        />
        <Image
          url="/assets/images/coach-2.jpeg"
          class="lg:w-[240px] w-3/5 h-[260px] object-cover rounded-xl shadow-sm drop-shadow-md"
        />
      </div>
    </div>
    <div class="lg:w-3/5 w-full">
      <p class="uppercase mb-1">Are you looking for a mentor</p>
      <MainHeading text="Coaches" class="uppercase" />
      <p class="text-black/45 font-light text-base mt-1 mb-6">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat.
      </p>
      <Button text="Explore More" class="w-fit"/>
    </div>
  </div>
</template>
