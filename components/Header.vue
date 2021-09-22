<template>
  <div class="fixed inset-x-0 bg-transparent z-10">
    <div class="w-full max-w-6xl mx-auto">
      <div
        class="flex justify-between items-center md:justify-start md:space-x-10 h-16"
      >
        <div class="flex justify-start lg:w-0 lg:flex-1">
          <nuxt-link to="/" class="">
            <span class="sr-only">SuppEd</span>
            <div class=" my-auto font-bold text-lg text-white">LIGHT ENGINEERING</div>
          </nuxt-link>
        </div>
        <div class="-mr-2 -my-2 md:hidden">
          <button
            @click="()=>open=true"
            type="button"
            class="bg-white rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
            aria-expanded="false"
          >
            <span class="sr-only">Open menu</span>
            <!-- Heroicon name: outline/menu -->
            <svg
              class="h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </button>
        </div>
        <div class="hidden md:flex items-center justify-end md:flex-1 lg:w-0 space-x-4">
          <div
            class="whitespace-nowrap text-sm font-bold uppercase text-white flex space-x-4 items-center px-2"
          >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-yellow-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
            </svg>
            <div>
                <div>Call Us</div>
                <p class=" text-xs font-semibold">+233 571 040 797</p>
            </div>
          </div>
          <div
            class="whitespace-nowrap text-sm font-bold uppercase border-l-2 border-white text-white px-2 flex space-x-4 items-center"
          >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-yellow-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 19v-8.93a2 2 0 01.89-1.664l7-4.666a2 2 0 012.22 0l7 4.666A2 2 0 0121 10.07V19M3 19a2 2 0 002 2h14a2 2 0 002-2M3 19l6.75-4.5M21 19l-6.75-4.5M3 10l6.75 4.5M21 10l-6.75 4.5m0 0l-1.14.76a2 2 0 01-2.22 0l-1.14-.76" />
            </svg>
            <div>
                <div>E-mail</div>
                <p class=" text-xs font-semibold lowercase">lightengineering@gmail.com</p>
            </div>
          </div>
          <div
            class="whitespace-nowrap text-sm font-bold uppercase border-l-2 border-white px-2 text-white flex space-x-4 items-center"
          >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-yellow-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
            <div>
                <div>Working hours</div>
                <p class=" text-xs font-semibold">Mon-Fir 11AM-19AM</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!--
    Mobile menu, show/hide based on mobile menu state.

    Entering: "duration-200 ease-out"
      From: "opacity-0 scale-95"
      To: "opacity-100 scale-100"
    Leaving: "duration-100 ease-in"
      From: "opacity-100 scale-100"
      To: "opacity-0 scale-95"
  -->
    <div
      class="absolute top-0 inset-x-0 p-2 transition transform origin-top-right md:hidden"
      v-if="open"
    >
      <div
        class="rounded-lg shadow-md ring-1 ring-black ring-opacity-5 bg-white divide-y-2 divide-gray-50"
      >
        <div class="pt-5 pb-6 px-5">
          <div class="flex items-center justify-between">
            <div class="flex justify-start lg:w-0 lg:flex-1">
              <nuxt-link to="/" class=" flex space-x-2">
                <span class="sr-only">SuppEd</span>
                <img
                  class="h-8 w-auto sm:h-10"
                  src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg"
                  alt=""
                />
                <div class=" my-auto font-bold text-lg">Supp<span class=" text-indigo-600">Ed</span></div>
              </nuxt-link>
            </div>
            <div class="-mr-2">
              <button
                @click="()=>open=false"
                type="button"
                class="bg-white rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
              >
                <span class="sr-only">Close menu</span>
                <svg
                  class="h-6 w-6"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  aria-hidden="true"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M6 18L18 6M6 6l12 12"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
        <div class="py-6 px-5 space-y-6">
          <div>
            <nuxt-link
              to="/parent/auth/guardian-information"
              class="w-full flex items-center justify-center px-4 py-2 border border-transparent rounded-md shadow-sm text-base font-medium text-white bg-indigo-600 hover:bg-indigo-700"
            >
              Sign up
            </nuxt-link>
            <p class="mt-6 text-center text-base font-medium text-gray-500">
              Existing customer?
              <nuxt-link to="/login" class="text-indigo-600 hover:text-indigo-500">
                Sign in
              </nuxt-link>
            </p>
            <div class="mt-6 text-center text-base font-medium text-gray-500">
            <nuxt-link to="/tutor/auth/sign-up" >
              Teach on SuppEd
            </nuxt-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      open:false
    }
  }
};
</script>

<style></style>
