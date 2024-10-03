<script setup>
import Image from "../Image.vue";
import MainHeading from "../MainHeading.vue";

const trainers = [
  {
    id: 1,
    image: "/assets/images/instructor-1.jpeg",
    name: "John Doe",
    bio: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
  },
  {
    id: 2,
    image: "/assets/images/instructor-3.jpeg",
    name: "Sara Safari",
    bio: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
  },
  {
    id: 3,
    image: "/assets/images/instructor-2.jpeg",
    name: "David Anders",
    bio: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
  },
];
</script>

<template>
  <div class="wrapper py-12">
    <MainHeading text="Meet Our Trainers" class="text-center" />
    <p
      class="text-base text-black/50 font-light text-center max-w-[540px] mx-auto"
    >
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua.
    </p>

    <div class="grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 gap-4 mt-16">
      <div v-for="item in trainers" :key="item.id" class="group relative">
        <Image
          :url="item.image"
          class="lg:w-72 w-full rounded-2xl mx-auto h-80 object-cover shadow-md drop-shadow-lg group-hover:blur-sm"
        />
        <div
          class="absolute inset-0 bg-black/55 lg:w-72 w-full mx-auto text-white p-4 rounded-2xl opacity-0 invisible transition-all ease-in-out duration-500 group-hover:opacity-100 group-hover:visible group-hover:h-full h-0"
        >
          <h4 class="text-2xl font-semibold mb-3">{{ item.name }}</h4>
          <p class="text-sm font-light text-white/90">{{ item.bio }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
