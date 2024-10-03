<script setup>
import Image from "../Image.vue";
import MainHeading from "../MainHeading.vue";

const data = [
  {
    icon: "/assets/images/glove.png",
    title: "Trainer Qualifications",
    desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore",
  },
  {
    icon: "/assets/images/dumbbell.png",
    title: "Facility Amenities",
    desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore",
  },
  {
    icon: "/assets/images/money.png",
    title: "Membership Cost",
    desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore",
  },
  {
    icon: "/assets/images/time.png",
    title: "Operation Hours",
    desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore",
  },
];
</script>

<template>
  <div class="py-14 wrapper">
    <MainHeading text="Why Choose Us" className="text-center pt-2" />
    <p
      class="text-lg text-black/40 font-light text-center md:px-20 px-6 mx-auto pt-1.5"
    >
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
      veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
      commodo consequat.
    </p>

    <div class="lg:flex lg:flex-row flex-col items-center gap-4 mt-16">
      <div class="lg:w-3/5 w-full flex-col flex gap-6 lg:pb-0 pb-12">
        <div class="grid md:grid-cols-2 grid-cols-1 md:gap-4 gap-8">
          <div v-for="(item, index) in data" :key="index" class="flex gap-4">
            <div class="size-10 min-w-10 rounded-full bg-[#1f1f1f] flex items-center justify-center">
              <Image :url="item.icon" class="size-6 object-contain"/>
            </div>
            <div>
              <h2 class="text-[#353535] font-semibold text-2xl mb-2">
                {{ item.title }}
              </h2>
              <p class="text-base text-black/50 font-light">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="lg:w-2/5 w-full">
        <div class="grid sm:grid-cols-2 grid-cols-1 items-stretch gap-4">
          <div class="flex flex-col gap-4">
            <div>
              <Image
                url="/assets/images/gym-1.png"
                class="w-full h-auto object-contain"
              />
            </div>
            <div>
              <Image
                url="/assets/images/gym-2.png"
                class="w-full h-auto object-contain"
              />
            </div>
          </div>
          <div>
            <Image url="/assets/images/gym-3.png" class="w-full h-auto" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
