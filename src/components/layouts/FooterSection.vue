<script setup>
import Image from "../Image.vue";
</script>

<template>
  <div class="wrapper py-16">
    <div class="grid md:grid-cols-3 grid-cols-1 gap-4">
      <div>
        <Image url="/assets/images/logo.png" class="w-44 h-auto" />
        <p class="text-[#919191] pt-4">
          Whether you’re curling up with a good book or hosting a festive
          holiday gathering, a fireplace makes every moment feel special and
          warm.
        </p>
      </div>
      <div class="md:mx-auto md:pt-0 pt-8">
        <h3 class="text-black/80 font-bold text-2xl">Social Media</h3>
        <div class="flex flex-col gap-6 pt-10">
          <a
            href="#"
            class="text-[#919191] font-medium text-lg flex items-stretch gap-2"
          >
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g opacity="0.4">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M6.18182 10.3333C5.20406 10.3333 5 10.5252 5 11.4444V13.1111C5 14.0304 5.20406 14.2222 6.18182 14.2222H8.54545V20.8889C8.54545 21.8081 8.74951 22 9.72727 22H12.0909C13.0687 22 13.2727 21.8081 13.2727 20.8889V14.2222H15.9267C16.6683 14.2222 16.8594 14.0867 17.0631 13.4164L17.5696 11.7497C17.9185 10.6014 17.7035 10.3333 16.4332 10.3333H13.2727V7.55556C13.2727 6.94191 13.8018 6.44444 14.4545 6.44444H17.8182C18.7959 6.44444 19 6.25259 19 5.33333V3.11111C19 2.19185 18.7959 2 17.8182 2H14.4545C11.191 2 8.54545 4.48731 8.54545 7.55556V10.3333H6.18182Z"
                  stroke="black"
                  stroke-width="1.8"
                  stroke-linejoin="round"
                />
              </g>
            </svg>

            Facebook</a
          >
          <a
            href="#"
            class="text-[#919191] font-medium text-lg flex items-stretch gap-2"
          >
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g opacity="0.4">
                <path
                  d="M2.5 12C2.5 7.52166 2.5 5.28249 3.89124 3.89124C5.28249 2.5 7.52166 2.5 12 2.5C16.4783 2.5 18.7175 2.5 20.1088 3.89124C21.5 5.28249 21.5 7.52166 21.5 12C21.5 16.4783 21.5 18.7175 20.1088 20.1088C18.7175 21.5 16.4783 21.5 12 21.5C7.52166 21.5 5.28249 21.5 3.89124 20.1088C2.5 18.7175 2.5 16.4783 2.5 12Z"
                  stroke="black"
                  stroke-width="1.8"
                  stroke-linejoin="round"
                />
                <path
                  d="M16.5 12C16.5 14.4853 14.4853 16.5 12 16.5C9.51472 16.5 7.5 14.4853 7.5 12C7.5 9.51472 9.51472 7.5 12 7.5C14.4853 7.5 16.5 9.51472 16.5 12Z"
                  stroke="black"
                  stroke-width="1.8"
                />
                <path
                  d="M17.5061 6.5H17.4971"
                  stroke="black"
                  stroke-width="1.8"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </g>
            </svg>

            Instagram</a
          >
          <a
            href="#"
            class="text-[#919191] font-medium text-lg flex items-stretch gap-2"
          >
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g opacity="0.4">
                <path
                  d="M4.5 9.5H4C3.05719 9.5 2.58579 9.5 2.29289 9.79289C2 10.0858 2 10.5572 2 11.5V20C2 20.9428 2 21.4142 2.29289 21.7071C2.58579 22 3.05719 22 4 22H4.5C5.44281 22 5.91421 22 6.20711 21.7071C6.5 21.4142 6.5 20.9428 6.5 20V11.5C6.5 10.5572 6.5 10.0858 6.20711 9.79289C5.91421 9.5 5.44281 9.5 4.5 9.5Z"
                  stroke="black"
                  stroke-width="1.8"
                />
                <path
                  d="M6.5 4.25C6.5 5.49264 5.49264 6.5 4.25 6.5C3.00736 6.5 2 5.49264 2 4.25C2 3.00736 3.00736 2 4.25 2C5.49264 2 6.5 3.00736 6.5 4.25Z"
                  stroke="black"
                  stroke-width="1.8"
                />
                <path
                  d="M12.326 9.5H11.5C10.5572 9.5 10.0858 9.5 9.79289 9.79289C9.5 10.0858 9.5 10.5572 9.5 11.5V20C9.5 20.9428 9.5 21.4142 9.79289 21.7071C10.0858 22 10.5572 22 11.5 22H12C12.9428 22 13.4142 22 13.7071 21.7071C14 21.4142 14 20.9428 14 20L14.0001 16.5001C14.0001 14.8433 14.5281 13.5001 16.0879 13.5001C16.8677 13.5001 17.5 14.1717 17.5 15.0001V19.5001C17.5 20.4429 17.5 20.9143 17.7929 21.2072C18.0857 21.5001 18.5572 21.5001 19.5 21.5001H19.9987C20.9413 21.5001 21.4126 21.5001 21.7055 21.2073C21.9984 20.9145 21.9985 20.4432 21.9987 19.5006L22.0001 14.0002C22.0001 11.515 19.6364 9.50024 17.2968 9.50024C15.9649 9.50024 14.7767 10.1531 14.0001 11.174C14 10.5439 14 10.2289 13.8632 9.995C13.7765 9.84686 13.6531 9.72353 13.505 9.63687C13.2711 9.5 12.9561 9.5 12.326 9.5Z"
                  stroke="black"
                  stroke-width="1.8"
                  stroke-linejoin="round"
                />
              </g>
            </svg>
            Linkedin</a
          >
        </div>
      </div>
      <div class="md:mx-auto">
        <h3 class="text-black/80 font-bold text-2xl pb-8 md:pt-0 pt-8">Location</h3>
        <div class="flex flex-col gap-6">
          <div class="flex items-center gap-4">
            <Image
              url="/assets/images/location.png"
              class="w-8 h-auto object-contain"
            />
            <div>
              <p class="text-[#919191] font-medium">Address:</p>
              <p class="text-[#919191]">13 Division st, New York, 16004</p>
            </div>
          </div>
          <div class="flex items-center gap-4">
            <Image
              url="/assets/images/phone.png"
              class="w-8 h-auto object-contain"
            />
            <div>
              <p class="text-[#919191] font-medium">Phone:</p>
              <p class="text-[#919191]">+1 - 5852826417</p>
            </div>
          </div>
          <div class="flex items-center gap-4">
            <Image
              url="/assets/images/clock.png"
              class="w-8 h-auto object-contain"
            />
            <div>
              <p class="text-[#919191] font-medium">Working Hours:</p>
              <p class="text-[#919191]">Mon-Sat: 6am – 11pm</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
