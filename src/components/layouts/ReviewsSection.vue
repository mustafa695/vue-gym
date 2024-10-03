<script setup>
import { Carousel, Navigation, Pagination, Slide } from "vue3-carousel";
import Button from "../Button.vue";
import Image from "../Image.vue";
import MainHeading from "../MainHeading.vue";
import "vue3-carousel/dist/carousel.css";

const reviews = [
  {
    name: "Sarah Thompson",
    review:
      "Joining this gym has been one of the best decisions I've made for my fitness journey. The equipment is top-notch and well-maintained, making my workouts enjoyable and efficient. The trainers are knowledgeable and genuinely care about helping you reach your goals. Plus, the community is welcoming and supportive, which keeps me motivated to show up every day!",
  },
  {
    name: "Jake Wilson",
    review:
      "This gym has a fantastic atmosphere! The staff is friendly, and the classes are diverse and engaging. I particularly love the spin classes; the energy is contagious. It’s the perfect place to stay fit and meet like-minded people.",
  },
  {
    name: "Megan Davis",
    review:
      "I was nervous about joining a gym, but the supportive community here made all the difference. The personal trainers take the time to understand your goals and create a customized plan. I’ve seen amazing results in just a few months!",
  },
  {
    name: "David Kim",
    review:
      "The facilities are clean, and there's a great variety of equipment. I appreciate that they have everything from weights to cardio machines. I’ve also enjoyed the yoga classes, which help me unwind after a tough week.",
  },
  {
    name: "Emily Nguyen",
    review:
      "I love the flexibility this gym offers! With extended hours and numerous class options, I can easily fit workouts into my busy schedule. The staff is always ready to help, making it a pleasant environment.",
  },
  {
    name: "Chris Brown",
    review:
      "While I initially joined for the equipment, I’ve fallen in love with the community vibe here. Everyone is encouraging, and the group classes are fun and challenging. It’s become more than just a gym; it feels like a second home!",
  },
  {
    name: "Laura Martinez",
    review:
      "The variety of classes is incredible! From kickboxing to Pilates, there's something for everyone. I appreciate that the instructors are passionate and provide modifications for all fitness levels.",
  },
  {
    name: "Kevin Patel",
    review:
      "I’m impressed with how clean and organized the gym is. The management clearly prioritizes hygiene, especially with the current health concerns. I feel safe and comfortable working out here, which is so important.",
  },
  {
    name: "Jessica Lee",
    review:
      "As someone who’s struggled with motivation, this gym has been a game changer for me. The friendly atmosphere and supportive trainers have helped me push through barriers I thought I’d never overcome.",
  },
  {
    name: "Ryan Johnson",
    review:
      "I've tried several gyms, but this one stands out due to its community feel. Everyone encourages each other, and the events they host make it easy to connect with fellow members. It's a great place to be!",
  },
];
</script>

<template>
  <div class="py-16 wrapper">
    <div class="flex sm:flex-row flex-col sm:pb-0 pb-6 items-center justify-between gap-4">
      <div>
        <p class="text-black/50">Reviews</p>
        <MainHeading text="From You" class="uppercase" />
      </div>
      <Button text="+ Give Review" />
    </div>
    <div class="grid lg:grid-cols-3 grid-cols-1 gap-4">
      <div>
        <Image
          url="/assets/images/profiles.png"
          class="lg:w-full w-9/12 lg:mx-0 mx-auto h-auto object-contain"
        />
      </div>
      <div class="col-span-2">
        <Carousel :items-to-show="1.5">
          <Slide v-for="(item, index) in reviews" :key="index">
            <div class="border border-black/40 rounded-2xl w-[450px]">
              <Image
                url="/assets/images/logo.png"
                class="ml-auto w-[86px] h-auto object-contain px-4 pt-3"
              />
              <div class="px-4 pb-4 -mt-1">
                <h3 class="text-[#1a1a1a] sm:text-2xl text-lg pb-3.5 font-semibold">
                  {{ item.name }}
                </h3>
                <svg
                  width="120"
                  height="20"
                  viewBox="0 0 120 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g opacity="0.8">
                    <path
                      d="M11.7276 1.44418L13.4874 4.99288C13.7274 5.48687 14.3673 5.9607 14.9073 6.05143L18.0969 6.58575C20.1367 6.92853 20.6167 8.4206 19.1468 9.8925L16.6671 12.3927C16.2471 12.8161 16.0172 13.6327 16.1471 14.2175L16.8571 17.3125C17.417 19.7623 16.1271 20.71 13.9774 19.4296L10.9877 17.6452C10.4478 17.3226 9.5579 17.3226 9.0079 17.6452L6.01827 19.4296C3.8785 20.71 2.57865 19.7522 3.13859 17.3125L3.84851 14.2175C3.97849 13.6327 3.74852 12.8161 3.32856 12.3927L0.848839 9.8925C-0.611001 8.4206 -0.14105 6.92853 1.89872 6.58575L5.08837 6.05143C5.61831 5.9607 6.25824 5.48687 6.49821 4.99288L8.258 1.44418C9.2179 -0.481393 10.7777 -0.481393 11.7276 1.44418Z"
                      fill="black"
                    />
                    <path
                      d="M36.7276 1.44418L38.4874 4.99288C38.7274 5.48687 39.3673 5.9607 39.9073 6.05143L43.0969 6.58575C45.1367 6.92853 45.6167 8.4206 44.1468 9.8925L41.6671 12.3927C41.2471 12.8161 41.0172 13.6327 41.1471 14.2175L41.8571 17.3125C42.417 19.7623 41.1271 20.71 38.9774 19.4296L35.9877 17.6452C35.4478 17.3226 34.5579 17.3226 34.0079 17.6452L31.0183 19.4296C28.8785 20.71 27.5786 19.7522 28.1386 17.3125L28.8485 14.2175C28.9785 13.6327 28.7485 12.8161 28.3286 12.3927L25.8488 9.8925C24.389 8.4206 24.8589 6.92853 26.8987 6.58575L30.0884 6.05143C30.6183 5.9607 31.2582 5.48687 31.4982 4.99288L33.258 1.44418C34.2179 -0.481393 35.7777 -0.481393 36.7276 1.44418Z"
                      fill="black"
                    />
                    <path
                      d="M61.7276 1.44418L63.4874 4.99288C63.7274 5.48687 64.3673 5.9607 64.9073 6.05143L68.0969 6.58575C70.1367 6.92853 70.6167 8.4206 69.1468 9.8925L66.6671 12.3927C66.2471 12.8161 66.0172 13.6327 66.1471 14.2175L66.8571 17.3125C67.417 19.7623 66.1271 20.71 63.9774 19.4296L60.9877 17.6452C60.4478 17.3226 59.5579 17.3226 59.0079 17.6452L56.0183 19.4296C53.8785 20.71 52.5786 19.7522 53.1386 17.3125L53.8485 14.2175C53.9785 13.6327 53.7485 12.8161 53.3286 12.3927L50.8488 9.8925C49.389 8.4206 49.8589 6.92853 51.8987 6.58575L55.0884 6.05143C55.6183 5.9607 56.2582 5.48687 56.4982 4.99288L58.258 1.44418C59.2179 -0.481393 60.7777 -0.481393 61.7276 1.44418Z"
                      fill="black"
                    />
                    <path
                      d="M86.7276 1.44418L88.4874 4.99288C88.7274 5.48687 89.3673 5.9607 89.9073 6.05143L93.0969 6.58575C95.1367 6.92853 95.6167 8.4206 94.1468 9.8925L91.6671 12.3927C91.2471 12.8161 91.0172 13.6327 91.1471 14.2175L91.8571 17.3125C92.417 19.7623 91.1271 20.71 88.9774 19.4296L85.9877 17.6452C85.4478 17.3226 84.5579 17.3226 84.0079 17.6452L81.0183 19.4296C78.8785 20.71 77.5786 19.7522 78.1386 17.3125L78.8485 14.2175C78.9785 13.6327 78.7485 12.8161 78.3286 12.3927L75.8488 9.8925C74.389 8.4206 74.8589 6.92853 76.8987 6.58575L80.0884 6.05143C80.6183 5.9607 81.2582 5.48687 81.4982 4.99288L83.258 1.44418C84.2179 -0.481393 85.7777 -0.481393 86.7276 1.44418Z"
                      fill="black"
                    />
                    <path
                      opacity="0.2"
                      d="M111.728 1.44418L113.487 4.99288C113.727 5.48687 114.367 5.9607 114.907 6.05143L118.097 6.58575C120.137 6.92853 120.617 8.4206 119.147 9.8925L116.667 12.3927C116.247 12.8161 116.017 13.6327 116.147 14.2175L116.857 17.3125C117.417 19.7623 116.127 20.71 113.977 19.4296L110.988 17.6452C110.448 17.3226 109.558 17.3226 109.008 17.6452L106.018 19.4296C103.878 20.71 102.579 19.7522 103.139 17.3125L103.849 14.2175C103.978 13.6327 103.749 12.8161 103.329 12.3927L100.849 9.8925C99.389 8.4206 99.8589 6.92853 101.899 6.58575L105.088 6.05143C105.618 5.9607 106.258 5.48687 106.498 4.99288L108.258 1.44418C109.218 -0.481393 110.778 -0.481393 111.728 1.44418Z"
                      fill="black"
                    />
                  </g>
                </svg>
                <p
                  class="text-[#333333] font-medium sm:text-lg text-sm leading-6 pt-4 text-left max-h-[10rem] overflow-hidden overflow-ellipsis"
                  style="
                    display: -webkit-box;
                    -webkit-box-orient: vertical;
                    -webkit-line-clamp: 5;
                  "
                >
                  {{ item.review }}
                </p>
              </div>
            </div>
          </Slide>

          <template #addons>
            <Pagination />
          </template>
        </Carousel>
      </div>
    </div>
  </div>
</template>
