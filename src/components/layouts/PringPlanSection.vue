<script setup>
import Button from "../Button.vue";
import MainHeading from "../MainHeading.vue";

const paymentMethods = [
  {
    id: 1,
    type: "Begginer Plan",
    price: "05",
    plan: "Month",
  },
  {
    id: 2,
    type: "Premium Plan",
    price: "15",
    plan: "Month",
  },
  {
    id: 3,
    type: "Expert Plan",
    price: "20",
    plan: "Month",
  },
];
</script>

<template>
  <div class="wrapper py-8">
    <div class="flex justify-between gap-4 pb-7">
      <div>
        <p class="text-black/50">Pricing plan</p>
        <MainHeading text="Join Today" class="uppercase" />
      </div>
    </div>
    <div class="grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 gap-6 px-6">
      <div
        v-for="item in paymentMethods"
        :key="item.id"
        class="w-full shadow-xl drop-shadow-xl bg-white shadow-[#ddd] p-6 rounded-2xl relative group"
      >
        <p class="text-base text-black group-hover:text-[#bcbcbc] font-medium">
          {{ item.type }}
        </p>
        <h2
          class="felx items-end text-[#1a1a1a] group-hover:text-[#e9e9e9] text-[52px] font-semibold"
        >
          ${{ item.price }}
          <span
            class="text-sm font-medium text-black group-hover:text-[#e9e9e9] -ml-1"
            >/ {{ item.plan }}</span
          >
        </h2>
        <p
          class="text-black/70 group-hover:text-[#8f8f8f] font-light text-sm pb-6 pt-4"
        >
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut
        </p>
        <div class="mb-14 flex flex-col gap-2">
          <div
            class="flex items-center gap-3"
            :key="index"
            v-for="(_i, index) in Array.from({ length: 5 })"
          >
            <svg
              width="20"
              height="20"
              viewBox="0 0 20 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g opacity="0.4">
                <circle opacity="0.7" cx="10" cy="10" r="10"  class="fill-[#1F1F1F] group-hover:fill-[#acacac]" />
                <path
                  d="M6.49902 11L7.70622 12.2072C8.00394 12.5049 8.48835 12.4993 8.77906 12.1947L13.499 7.25"
                  stroke="white"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </g>
            </svg>
            <p class="text-[#666666] group-hover:text-[#a5a5a5]">
              Lorem ipsum dolor sit amit.
            </p>
          </div>
        </div>
        <Button
          text="Choose Plan"
          class="w-full !py-3.5 group-hover:text-black group-hover:bg-white"
        />
        <div
          class="absolute inset-0 bg-black rounded-2xl -z-10 group-hover:opacity-100 group-hover:visible opacity-0 invisible transition-all duration-500 ease-in-out"
        ></div>
      </div>
    </div>
  </div>
</template>
